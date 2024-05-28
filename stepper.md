# React-form-stepper
`import {Step, Stepper} from 'react-form-stepper';`

## main
```
<Stepper activeStep={x} connectorStateColors={true} styleConfig={StepStyleDTO}
                     connectorStyleConfig={ConnectorStyleProps}>
    <Step label="x1"/>
    <Step label="x2"/>
    <Step label="x3"/>
    <Step label="x4"/>
</Stepper>
```

## Options
```
const ConnectorStyleProps = {
    disabledColor: 'rgba(143,143,143,0.44)',
    activeColor: '#ffffff',
    completedColor: '#ffffff'
}

const StepStyleDTO = {
    activeBgColor: '#1271c8',
    activeTextColor: '#fff',
    inactiveBgColor: 'rgba(106,105,105,0.94)',
    inactiveTextColor: '#ddd8d8',
    completedBgColor: '#2dcc1a',
    completedTextColor: '#ffffff',
    size: '2.5em'
}
```
