# react-otp-input

A fully customizable, one-time password input component for the web built with React.

## Installation

To install the latest stable version:
```
npm install --save react-otp-input
```

Basic usage:
```javascript
import React, { Component } from 'react';
import OtpInput from 'react-otp-input';

export default class App extends Component {
  render() {
    return (
      <div>
        <OtpInputs 
          onChange={otp => console.log(otp)}
          numInputs={6}
          separator={<span>-<span>}
        />
      </div>
    )
  }
}
```

## API

<table>
  <tr>
    <th>Name<br></th>
    <th>Type</th>
    <th>Required</th>
    <th>Default</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>numInputs</td>
    <td>number</td>
    <td>true</td>
    <td>4</td>
    <td>Number of OTP inputs to be rendered.</td>
  </tr>
  <tr>
    <td>onChange</td>
    <td>function</td>
    <td>true</td>
    <td>console.log</td>
    <td>Returns OTP code typed in inputs.</td>
  </tr>
  <tr>
    <td>separator</td>
    <td>component<br></td>
    <td>false</td>
    <td></td>
    <td>Provide a custom separator between inputs by passing a component. For instance, <code>&lt;span&gt;-&lt;/span&gt;</code> would add <code>-</code> between each input</td>
  </tr>
  <tr>
    <td>containerStyle</td>
    <td>style (object)</td>
    <td>false</td>
    <td>none</td>
    <td>Style applied to container of inputs.</td>
  </tr>
  <tr>
    <td>inputStyle</td>
    <td>style (object)</td>
    <td>false</td>
    <td>none</td>
    <td>Style applied to each input.</td>
  </tr>
</table>                         

## Checklist

- [ ] Add styling support for states including focus/disabled
- [ ] Travis CI, Codecov
- [ ] Write tests

## Contributing

Feel free to open issues and pull requests!

## License

MIT