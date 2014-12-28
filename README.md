jquery 粒子随机连接动态背景
==============

动态粒子随机连接的背景效果，包含鼠标经过背景时候的反响经过和移动设备的滑动效果。
如果运行在高级浏览器，支持canvas

[DEMO地址](https://jnicol.github.io/particleground)

## 使用方法

    $('#your-element').particleground();

## 选项

你可以通过粘贴下面的示例，来熟悉了解选项功能。

这里有一个设置粒子和连接线条颜色的示例：

    $('#your-element').particleground({
        dotColor: '#ff0000',
        lineColor: '#ff0000'
    });

下面是所有选项的功能清单和主要的参数：

### minSpeedX

    0.1

### maxSpeedX

    0.7

### minSpeedY

    0.1

### maxSpeedY

    0.7

### directionX

    'center'

center'`, `'left' or `'right'`. `'center'` 这几个参数是设置粒子圆圈的碰撞的边缘

### directionY

    'center'

Can be one of `'center'`, `'up'` or `'down'`. `'center'` means that the dots will bounce off the edges of the canvas.

### density

    10000

设置生产粒子圆圈的数量：可以理解尾，一个粒子有多少个像素

### dotColor

    '#666666'

### lineColor

    '#666666'

### particleRadius

    7

粒子的半径

### lineWidth

    1

### curvedLines

    false

### proximity

    100

How close two dots need to be, in pixels, before they join.

### parallax

    true

### parallaxMultiplier

    5

The lower the number, the more extreme the parallax effect wil be.

### onInit

    function() {}

A callback executed after Particleground initializes.

### onDestroy

    function() {}

A callback executed after Particleground is destroyed.

## Methods

### pause

Pauses the particle system.

    $('#your-element').particlegound('pause');

### start

Restarts the particle system if you previously paused it.

    $('#your-element').particlegound('start');

### destroy

Removes the plugin from your element.

    $('#your-element').particlegound('destroy');

## Credits

Particleground was inspired by http://requestlab.fr/ and http://disruptivebydesign.com/ 
