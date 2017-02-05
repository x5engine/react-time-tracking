# Vivid Trace [![CircleCI](https://circleci.com/gh/tuanngominh/vivid-trace.svg?style=svg)](https://circleci.com/gh/tuanngominh/vivid-trace) [![codecov](https://codecov.io/gh/tuanngominh/vivid-trace/branch/master/graph/badge.svg)](https://codecov.io/gh/tuanngominh/vivid-trace)

Time tracking app on [React](https://facebook.github.io/react/) ([demo](https://vivid-trace.firebaseapp.com/)).

# Tech stack
Web application based on React (clientside) and Firebase (serverside)

React requirement:
- [x] Authencation
- [x] Form processing
- [x] Responsive
- [x] Unit test
- [x] Continous integration: circleci.com, codecov.io

# Requirement
Just try to build the death simple version of time tracking
- [x] Signup using email
- [x] Login, logout, forgot password

- Can add time entry
- Can track time spent on time entry and stop a time entry tracking
- Can list time entries
- Delete time entry

- Add tag to time entry
- CRUD tag

- Dashboard
- Can view report and visualized chart: detail chart, summary chart

- User profile

Low priority
- Signup using google, facebook

# Enzyme
Simulate `onClick` event in `shallow` ([github](https://github.com/airbnb/enzyme/issues/323#issuecomment-210039710))
```js
const componentWrapper = shallow(<Component />)
componentWrapper.simulate('click', { preventDefault() {} })
```

Simulate change event in [material-ui's TextField](http://www.material-ui.com/#/components/text-field) ([github](https://github.com/airbnb/enzyme/issues/364#issuecomment-217475038))
```js
const input = wrapper.find('input[name="text"]')
input.node.value = "newvalue"
input.simulate('change', input)
```