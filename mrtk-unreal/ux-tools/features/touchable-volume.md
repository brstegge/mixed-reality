---
title: Touchable volume
description: Guide to touchable volume resources and techniques in UXT.
author: luis-valverde-ms
ms.author: luval
ms.date: 08/25/2020
ms.localizationpriority: high
keywords: Unreal, Unreal Engine, UE4, HoloLens, HoloLens 2, Mixed Reality, development, MRTK, UXT, UX Tools, Manipulator Component, direct manipulation
---

# Touchable volume

The touchable volume component allows the user to interact with an object by touching it.

![Simulated hands interacting with touchable volume component](images/TouchableVolume/Example.gif)

## Usage

Create a `UxtTouchableVolumeComponent` on an Actor. By default, the volume will trigger events when the user interacts with any primitive on the actor. The can be configured by populating the _Touchable Primitives_ set with the primitives that should trigger events, which will limit interaction to only the primitives contained in the set.

## Events

The touchable volume generates several events that can be used to drive interactions:

- **OnBeginFocus**: Event raised when a pointer starts focusing the touchable volume.
- **OnUpdateFocus**: Event raised when a focusing pointer updates.
- **OnEndFocus**: Event raised when a pointer ends focusing the touchable volume.
- **OnBeginPoke**: Event raised when a pointer starts poking the touchable volume.
- **OnUpdatePoke**: Event raised while a pointer is poking the touchable volume.
- **OnEndPoke**: Event raised when a pointer ends poking the touchable volume.
- **OnVolumeEnabled**: Event raised when the volume is enabled.
- **OnVolumeDisabled**: Event raised when the volume is disabled.
