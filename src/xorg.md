# Xorg

X servers, X clients, [X11 protocol](https://www.x.org/releases/current/doc/xproto/x11protocol.html), [Xorg](http://cgit.freedesktop.org/xorg/xserver) is an implementation.

[Xlib](http://www.x.org/releases/current/doc/libX11/libX11/libX11.html) and [xcb](xcb.freedesktop.org) реализуют протокол X11.

Некоторые важные кусочки протокола:
* [Expose](http://www.x.org/releases/current/doc/xproto/x11protocol.html#events:Expose) просит у клиента нарисовать какой-нибудь кусочек окна, прямоугольничек. Например, при перемещении у окна открылась часть, которая была скрыта, и ее нужно прорисовать.

region это структура данных, которая представляет куски окон в виде прямоугольников, чтобы как-то хранить видимые части окон, что видно а что нет, и при этом экономить память (битовая маска пикселей занимает слишком большой объем памяти).

Xorg и cairo используют одну и ту же реализацию регионов из библиотеки [pixman](http://www.pixman.org/).

Pixmap это представление набора пикселей (например, картинки) на сервере. Чтобы не отправлять постоянно список пикселей при отрисовке регионов на сервер, можно отправить на сервер Pixmap и потом на него ссылаться.

Когда в окне нужно отрисовать новый кусок и метод Expose еще не отработал, есть три варианта отрисовки пока пустого места (задаются в свойствах окна):
- `background-pixel` - отрисовка фиксированным цветом
- `background-pixmap` - отрисовка загруженным pixmap'ом
- Делать ничего, оставить старые пиксели на месте пока не отработает Expose

Запрос [ReparentWindow](http://www.x.org/releases/current/doc/xproto/x11protocol.html#requests:ReparentWindow) назначает окну другого родителя. По умолчанию у всех окон родительское окно - корневое. Строить интерфейс на иерархии окон невыгодно, потому что каждое окно будет отрисовываться отдельно, для каждого будет отдельный запрос, и все будет лагать.

## Links

* [X Window System Basics](https://magcius.github.io/xplain/article/x-basics.html) with interactive examples
