---
layout: worksheet
title: Welcome
---

## Visual Reactive Programming with Bonsai

This training course will introduce you to the basic concepts of data acquisition and behavioural control using the [Bonsai](http://bonsai-rx.org/){:target="_blank"} visual programming language.

## Course Schedule

<table class="markdown-body">
    <thead>
        <tr>
            <th></th>
            <th align="center">Tuesday</th>
            <th align="center">Wednesday</th>
            <th align="center">Thursday</th>
            <th align="center">Friday</th>
            <th align="center">Monday</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Seminar</td>
            <td style="color:chocolate" align="center">Introduction to Bonsai</td>
            <td style="color:chocolate" align="center">Reactive Operators</td>
            <td style="color:chocolate" align="center">Higher Order Operators</td>
            <td style="color:chocolate" align="center">BonVision</td>
            <td style="color:chocolate" align="center">Wrap-up</td>
        </tr>
        <tr>
            <td>Recap</td>
            <td style="color:chocolate;background-color:bisque" align="center"></td>
            <td style="color:chocolate;background-color:bisque" align="center">Object Tracking</td>
            <td style="color:chocolate;background-color:bisque" align="center">Data Synchronization</td>
            <td style="color:chocolate;background-color:bisque" align="center">State Machines</td>
            <td style="color:chocolate;background-color:bisque" align="center"></td>
        </tr>
        <tr>
            <td>Workshop</td>
            <td style="color:cornflowerblue" align="center">Acquisition and Tracking</td>
            <td style="color:cornflowerblue" align="center">Closed-loop experiments</td>
            <td style="color:cornflowerblue" align="center">Operant behavior</td>
            <td style="color:cornflowerblue" align="center">Visual environments</td>
            <td style="color:cornflowerblue" align="center">Final projects</td>
        </tr>
    </tbody>
</table>

### Day 1 - Introduction to Bonsai
- Introduction to Bonsai. What is visual reactive programming?
- How to measure almost anything with Bonsai (from quantities to bytes).
- How to control almost anything with Bonsai (from bytes to effects).
- Real-time tracking of colored objects, moving objects and contrasting objects.
- Measuring behavior using voltages and an Arduino.

### Day 2 - Real-time closed-loop experiments
- Data synchronization and measuring closed-loop latency.
- Conditional effects. Triggering a stimulus based on video activity.
- Continuous feedback. Modulate stimulus intensity with speed or distance.
- Feedback stabilization. Record video centered around a moving object.
- Real-time markerless pose tracking using [Bonsai + DeepLabCut](https://github.com/bonsai-rx/deeplabcut){:target="_blank"} and [Bonsai + SLEAP](https://github.com/bonsai-rx/sleap){:target="_blank"}.

### Day 3 - Operant behavior tasks
- Creating dynamic observable sequences with higher-order operators.
- Modeling trial sequences: states, events, and side-effects.
- Driving state transitions with external inputs.
- Choice, timeouts and conditional logic. Building reaction time and Go/No-Go tasks.
- Best practices for composing complex workflows.

### Day 4 - Interactive visual environments
- Creating and controlling visual environments with [BonVision](https://bonvision.github.io/){:target="_blank"}.
- Building closed-loop virtual reality experiments.
- Combining real-time and non real-time logic.
- Building variable trial structures.
- Logging stimulus and response outcomes.

### Day 5 - Wrap-up
- How to extend Bonsai with scripting.
- Reproducible deployment and versioning of experiments.
- Interfacing Bonsai with Python and MATLAB.
- Bonsai hackathon and project presentations.
- Closing remarks.