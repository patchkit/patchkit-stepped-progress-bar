# Stepped Progress Bar

Component from [PatchKit](https://github.com/ssbc/patchkit).

## Usage

```jsx
import SteppedProgressBar from 'patchkit-stepped-progress-bar'
```

3 steps:

```jsx
<SteppedProgressBar num={3} current={0} />
```

4 steps:

```jsx
<SteppedProgressBar num={4} current={0} />
```

Add the ability to click on past steps, to jump back:

```jsx
const onGotoStep = step => console.log('Going back to step', step)
<SteppedProgressBar num={3} current={0} canGoBack onClick={onGotoStep} />
```

Label each step:

```jsx
<SteppedProgressBar labels={['first', 'second', 'third', 'fourth']} />
```

Use the .less file:

```less
@import "node_modules/patchkit-stepped-progress-bar/styles.less"
```

## License

GPL 3