# zp-react-redux-es6-standard

This is a simple colection of snippet for usage with React and Redux using ES6 and standard being using at Zeplyrplace.

## Features

[![JavaScript Style Guide](https://cdn.rawgit.com/standard/standard/master/badge.svg)](https://github.com/standard/standard)

| Command | Description |
| --- | --- |
| rcc | Create a React Component Class |

``` javascript
import React, { Component } from 'react'

export default class $1 extends Component {
  render () { 
    return (
      <div>$2</div>
    )
  }
}

```

| Command | Description |
| --- | --- |
| rcs | Create a React Component Stateless |

``` javascript
import React from 'react'

const $1 = () => {
  return (
    <div>$2</div>
  )
}

export default $1

```

| Command | Description |
| --- | --- |
| rccp | Create a React Component Class with PropTypes |

``` javascript
import React, { Component } from 'react'
import PropTypes from 'prop-types'

class $1 extends Component {
  render () {
    return (
      <div>$3</div>
    )
  }
}

$1.propTypes = {
  $2
}

export default $1


```

| Command | Description |
| --- | --- |
| rcsp | Create a React Component Class with PropTypes |

``` javascript
import React from 'react'
import PropTypes from 'prop-types'

const $1 = props => {
  return (
    <div>$3</div>
  )
}

$1.propTypes = {
  $2
}

export default $1

```

| Command | Description |
| --- | --- |
| rrcc | Create a Redux Container with connect and bindActionCreators |

``` javascript
import { bindActionCreators } from 'redux'
import { connect } from 'react-redux'

const mapStateToProps = (state) => ({ $1: state.$2 })
const mapDispatchToProps = (dispatch) => bindActionCreators($3, dispatch)

export default connect(mapStateToProps, mapDispatchToProps)($4)

```

| Command | Description |
| --- | --- |
| rrdc | Create a Redux Reducer |

``` javascript
export default (state = $1, action) => {
  switch (action.type) {
    case $2:
      $3
    default:
      return state
  }
}

```

| Command | Description |
| --- | --- |
| raf | Create a Redux action function |

``` javascript
export const $1 = '$1'

export const $2 = $3 => ({
  type: $1,
  $3
})

```

| Command | Description |
| --- | --- |
| rafr | Create a Redux action function with return |

``` javascript
export function $1 ($2) {
  return $3
}

```

![feature X](images/vsc-ext.gif)

> Why?: Many popular extensions utilize superfluous snippets. This is tiny with minimium requirements and the only one with correct Standard JS. 

## Requirements

```
npm install standard --save-dev
npm install prop-types --save
```

## Release Notes

### 1.0.0

Initial release of the main snippets usage at Zephyrplace

***
![Zephyrplace](https://avatars0.githubusercontent.com/u/17429557?s=200&v=4)