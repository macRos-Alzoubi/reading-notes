# CSS Transforms, Transitions, and Animations

## Transforms

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

## Transform Syntax

The actual syntax for the `transform` property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

  - ### i.g

  ```css
  div {
        -webkit-transform: scale(1.5);
        -moz-transform: scale(1.5);
        -o-transform: scale(1.5);
        transform: scale(1.5);
  }
  ```

Notice how the t`ransform` property includes multiple **vendor prefixes** to gain the best support across all browsers. The **un-prefixed** declaration comes last to overwrite the prefixed versions, should a browser fully support the transform property.


## 2D Transforms

Elements may be distorted, or transformed, on both a **two-dimensional** plane or a three-dimensional plane. Two-dimensional transforms work on the **x** and **y axes**, known as **horizontal** and **vertical** axes. T**hree-dimensional** transforms work on both the **x** and **y** axes, as well as the **z** axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.

  - ### 2D Rotate

    The `transform` property accepts a handful of different values. The `rotate` value provides the ability to rotate an element from `0` to `360` degrees. Using a positive value will rotate an element **clockwise**, and using a negative value will rotate the element **counterclockwise**.

    - #### i.g

    ```html
    <figure class="box-1">Box 1</figure>
    <figure class="box-2">Box 2</figure>
    ```

    ```css
        .box-1 {
    transform: rotate(20deg);
    }
    .box-2 {
    transform: rotate(-55deg);
    }
    ```

  - ### 2D Scale

    Using the `scale` value within the `transform` property allows you to change the appeared size of an element. The default `scale` value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

    - #### i.g

    ```html
        <figure class="box-1">Box 1</figure>
        <figure class="box-2">Box 2</figure>

    ```

    ```css
        .box-1 {
        transform: scale(.75);
        }
        .box-2 {
        transform: scale(1.25);
        }

    ```

  - ### 2D Translate

    The `translate` value works a bit like that of `relative` positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the `translateX` value will change the position of an element on the **horizontal** axis while using the `translateY` value will change the position of an element on the **vertical** axis.

    - #### i.g

    ```html
        <figure class="box-1">Box 1</figure>
        <figure class="box-2">Box 2</figure>
        <figure class="box-3">Box 3</figure>
    ```

    ```css
        .box-1 {
        transform: translateX(-10px);
        }
        .box-2 {
        transform: translateY(25%);
        }
        .box-3 {
        transform: translate(-10px, 25%);
        }
    ```

  - ### 2D Skew

    `skew`, is used to distort elements on the **horizontal** axis, **vertical** axis, or both. The syntax is very similar to that of the `scale` and `translate` values. Using the `skewX` value distorts an element on the **horizontal** axis while the `skewY` value distorts an element on the **vertical** axis. To distort an element on both axes the `skew` value is used, declaring the x axis value first, followed by a comma, and then the y axis value.%p

    The distance calculation of the `skew` value is measured in units of **degrees**. **Length measurements**, such as **pixels** or **percentages**, do not apply here.

    - #### i.g

    ```html
        <figure class="box-1">Box 1</figure>
        <figure class="box-2">Box 2</figure>
        <figure class="box-3">Box 3</figure>
    ```

    ```css
        .box-1 {
        transform: skewX(5deg);
        }
        .box-2 {
        transform: skewY(-20deg);
        }
        .box-3 {
        transform: skew(5deg, -20deg);
        }
    ```

## Combining Transforms

It is common for multiple `transforms` to be used at once, **rotating** and **scaling** the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of ***commas***.

Using multiple `transform` declarations ***will not work***, as each declaration will ***overwrite*** the one above it. The behavior in that case would be the same as if you were to set the height of an element numerous times.

  - #### i.g

    ```html
        <figure class="box-1">Box 1</figure>
        <figure class="box-2">Box 2</figure>
    ```

    ```css
        .box-1 {
        transform: rotate(25deg) scale(.75);
        }
        .box-2 {
        transform: skew(10deg, 20deg) translateX(20px);
        }
    ```

## Transform Origin

the **default** `transform` origin is the **dead center of an element, both 50% horizontally and 50% vertically**. To change this default origin position the `transform-origin` property may be used.

The `transform-origin` property can accept one or two values. **When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis**.

## Perspective

In order for **three-dimensional** transforms to work the elements need a `perspective` from which to `transform`. The `perspective` for each element**can be thought of as a vanishing point**, similar to that which can be seen in three-dimensional drawings.

The `perspective` of an element can be set in **two different ways**. One way **includes using the perspective value within the transform property on individual elements**, while the **other includes using the perspective property on the parent element residing over child elements being transformed**.

## Perspective Depth Value

The `perspective` value can be set as `none` or a **length measurement**. The none value turns off any perspective, while the length value will set the depth of the perspective. The higher the value, the further away the perspective appears, thus creating a fairly low intensity perspective and a small three-dimensional change. The lower the value the closer the perspective appears, thus creating a high intensity perspective and a large three-dimensional change.

## Transitions & Animations

One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

## Transitions

for a `transition` to take place, an element must have a change in **state**, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the `:hover, :focus, :active`, and `:target` **pseudo-classes**.

There are four `transition` related `properties` in total, including `transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay`. Not all of these are required to build a transition, with the first three are the most popular.

```css
    .box {
    background: #2db34a;
    transition-property: background;
    transition-duration: 1s;
    transition-timing-function: linear;
    }
    .box:hover {
    background: #ff7b29;
    }
```

## Transitional Property

The `transition-property` property determines exactly what **properties** will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, **only the properties identified within the `transition-property` value will be affected by any transitions**.

## Transition Duration

The `duration` in which a `transition` takes place is set using the `transition-duration` property. The value of this property can be set using general timing values, **including seconds (s)** and **milliseconds (ms)**. These timing values may also come in **fractional measurements, .2s** for example.

## Transition Timing

The `transition-timing-function` property is used to set the ***speed*** in which a transition will move. Knowing the duration from the `transition-duration` property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the `transition-timing-function` property include `linear`, `ease-in`, `ease-out`, and `ease-in-out`.

## Transition Delay

On top of declaring the `transition` property, `duration`, and **timing** function, you can also set a **delay** with the `transition-delay` property. The delay sets a time value, seconds or milliseconds, that determines how long a `transition` should be stalled before executing. As with all other `transition` properties, to delay numerous transitions, each delay can be declared as comma separated values.

## Animations

`Transitions` do a great job of building out visual interactions from **one state to another**, and are perfect for these kinds of s**ingle state changes**. However, when more control is required, transitions need to have multiple states. In return, this is where `animations` pick up where `transitions` leave off.

## Animations Keyframes

To set multiple points at which an element should undergo a transition, use the `@keyframes` rule. The `@keyframes` rule includes the `animation name`, any `animation breakpoints`, and the properties intended to be animated.

```css
    keyframes slide {
    0% {
        left: 0;
        top: 0;
    }
    50% {
        left: 244px;
        top: 100px;
    }
    100% {
        left: 488px;
        top: 0;
    }
    }

```

## Animation Name

Once the `keyframes` for an `animation` have been declared they need to be assigned to an element. To do so, the `animation-name` property is used with the animation name, identified from the `@keyframes` rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.

## Animation Duration, Timing Function, & Delay

Once you have declared the `animation-name` property on an element, animations behave similarly to `transitions`. They include a `duration`, `timing function`, and `delay` if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.

```css
    .stage:hover .ball {
    animation-name: slide;
    animation-duration: 2s;
    animation-timing-function: ease-in-out;
    animation-delay: .5s;
    }

```

## Animation Iteration

By default, `animations` run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the `animation-iteration-count` property may be used. Values for the `animation-iteration-count` property include either an **integer** or the **infinite** keyword. Using an integer will repeat the animation as many times as specified, while the **infinite** keyword will repeat the animation **indefinitely** in a **never ending fashion**.

## Animation Direction

On top of being able to set the number of times an animation repeats, you may also declare the direction an animation completes using the `animation-direction` property. Values for the animation-direction property include `normal`, `reverse`, `alternate`, and `alternate-reverse`.

## Animation Play State

The `animation-play-state` property allows an `animation` to be `played` or `paused` using the `running` and `paused` keyword values respectively. When you play a paused animation, it will resume running from its current state rather than starting from the very beginning again.

## Animation Fill Mode

The `animation-fill-mode` property **identifies how an element should be styled either before, after, or before and after** an animation is run. The `animation-fill-mode` property accepts four keyword values, including `none`, `forwards`, `backwards`, and `both`.

The `none` value will not apply any styles to an element before or after an `animation` has been run.

The `forwards` value will keep the styles declared within the last specified `keyframe`. These styles may, however, be affected by the `animation-direction` and `animation-iteration-count` property values, changing exactly where an animation ends.

The `backwards` value will apply the styles within the first specified `keyframe` as soon as being identified, before the animation has been run. This does include applying those styles during any time that may be set within an animation delay. The `backwards` value may also be affected by the `animation-direction` property value.

Lastly, the `both` value will apply the behaviors from both the forwards and backwards values.
