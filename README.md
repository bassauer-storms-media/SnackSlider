# SnackSlider
Snackslider is a simple slide show library that focuses on allowing to change options and images while running.
The source length of the snack slider is less than 300 lines, and it has a very simple structure.

## Feature

- No control button, only functions.
- Super smooth slide change.
- You can add and delete images while running a slide show smoothly.
- You can modify all options while running a slide show : mode, speed, etc...

## Dependency

- JQuery (3.1 or above)

## Tested browser

- Chrome 73
- Safari 12

## Usage

Please refer to the test folder.


````
<script>
        let slider;
        $(document).ready(function () {
            slider = new SnackSlider({
                selector: '.slider',
                mode: 'right',
                speed: 2000,
                pause: 3000,
                width: 320,
                height: 240,
                fit: 'cover',
                children: [
                    './rainbow.jpg',
                    './rio.jpg',
                    './spiral-staircase.jpg',
                ]
            });
        });
    </script>


</head>
<body>
    <div class="slider" style="width:640px;height:480px"></div>

````

## Options

| Option Name | Type | Default value | Description |
| ----------- | ---- | ------------- | ----------------------------------------------------------------------|
| selector    | string | -           | Required. JQuery selector pointing to the html element to include the slider. |
| mode        | string | 'right'     | One of 'right', 'left', 'top', 'bottom', 'fade'. Mode of slide show. |
| speed       | integer| 1000        | The amount of time it takes for an animation to change images. (ms) |
| pause       | integer| 4000        | The amount of time when the image is frozen. (ms) |
| width       | integer| 0           | If 0, width is parent element's width. |
| height      | integer| 0           | If 0, height is parent element's height. |
| fit         | string | 'cover'     | Value of css 'object-fit' for slide's img tag |
| background  | string | 'white'     | Value of css 'background-color' for slide's img tag |


## Changelog

**V1.0.1**
- Remove some bug. 

**V1.0.0**
- First commit.

## License

**MIT**

## Remarks

If you find that SnackSlider is useful, please support me with [a glass of beer :beer:](https://www.paypal.me/SeunghoYi). 
