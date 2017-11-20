# React Native TapTargetView
React Native Bridge for [KeepSafe/TapTargetView](https://github.com/KeepSafe/TapTargetView)

<img src="https://github.com/KeepSafe/TapTargetView/blob/master/.github/video.gif" width="280" height="498" alt="Video 1"/>

## Installation

- `$ npm install react-native-taptargetview --save`

- `$ react-native link react-native-taptargetview`

#### [Manual Installation](./Installation.md)

## API's

- TapTarget.forView: TapTarget
`
let tapTarget = TapTarget.forView(Button, {
    title: 'This is a target button 1',
    description: 'We have the best targets, believe me'
})

TapTargetView.ShowFor(tapTarget)
`

- TapTargetSequence
    - add(TapTarget)
    - remove(TapTarget)
    - removeAll
    - get(TapTarget)
    - getAll

`
let tapTargetSequence = new TapTargetSequence()
this.tapTargets.forEach(tapTarget => {
tapTargetSequence.add(tapTarget)
})

TapTargetView.ShowSequence(tapTargetSequence)
`

- TapTargetView
    - ShowFor(TapTarget)
    - ShowSequence(TapTargets)