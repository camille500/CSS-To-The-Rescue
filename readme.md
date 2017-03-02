# CSS-To-The-Rescue

This read me contains all documentation and annotations made during the course.
All sources I've used so far can be find at the bottom of this read me.

## Links to the Live Versions:
- [Week 1](https://camille500.github.io/CSS-To-The-Rescue/week1/)
- [Week 2](https://camille500.github.io/CSS-To-The-Rescue/week2/)
- [Week 3](https://camille500.github.io/CSS-To-The-Rescue/week3/)

## Annotations

Here you can find all the annotations I have made during the CSS To The Rescue course.

### CSS Secrets - Chapter 1

To get an better understanding of CSS, I've bought the book 'CSS Secrets' from Lea Verou. Here are the annotations I've made from the first chapter.

#### Best practices

- It's important to keep your code ***DRY***. If you follow this principle, your code gets better maintainable. It minimizes the amount of edits necessary to make a change.

- When values depend on each other, try to reflect their relationship in the code.
- Use relative measures units like ***EM's*** and ***%***.
- ***Inheritance*** corresponds to the computed value of the parent element. It can be used on almost every CSS property.
- Media query thresholds should not be dictated by specific devices, but by the design itself.

#### The :target selector

- The ***:target selector*** can be used to style an element that is targeted. Based on the hash in the url, the targeted element can be styled with CSS. The example below is a simple example of how its done.

```
<a href="#showDiv">Show the div</a>

<div id="showDiv>

	<h1>Here is the div</h1>

</div>
```

```
div {
	display: none;
}

div:target {
	display:block;
}
```

- In the example above the div is hidden by default. As soon as you click the link with href '#showDiv', the div with id 'showDiv' is targeted and the div becomes visible.

#### Vertical centring

- Sometimes you want to center something vertically on the page. That can be done easily using the example below.

```
main {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
}
```

- The main section is now vertically centered in the parent element. This could also be done with a div inside the main section for example.


### Sources
- http://getemoji.com/
- https://flatuicolors.com/
