---
layout: slides
title: Reactive Operators
permalink: /slides/reactive/
---

<section data-markdown data-separator="^\n---\n$" data-separator-vertical="^\n--\n$">
<script type="text/template">

![Bonsai](../../assets/images/bonsai-lettering.svg)

### Reactive Operators
[neurogears.org/vrp-2022](https://neurogears.org/vrp-2022)
<table style="width: 100%;">
  <tr>
    <th style="vertical-align: middle; width: 50%; height: 100px; padding-left: 100px">
      <img alt="NeuroGEARS" src="../../assets/images/neurogears.svg"/>
    </th>
    <th style="vertical-align: middle; width: 50%; height: 100px; align: right">
      <img alt="Cajal" src="../../assets/images/cajal.png"/>
    </th>
  </tr>
</table>

---

### Outline

* Recap
* Reactive Operators

---

<!-- .element: data-transition="default none" -->
#### A metaphor for observable sequences

<img alt="Nasa twitter account" src="../../assets/images/nasatwitter.jpg" width="400"/>

--

<!-- .element: data-transition="none" -->
#### A metaphor for observable sequences

<img alt="Webcam twitter account" src="../../assets/images/webcamtwitter.jpg" width="400"/>

---

<!-- .element: data-transition="default none" -->
![Workflow](../../assets/images/cameracapture.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/framepicker-marblecanvas.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="default none" -->
![Workflow](../../assets/images/graycam.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/graycam-marble.svg)
<!-- .element: class="fragment" style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="default none" -->
![Workflow](../../assets/images/framepicker-key.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/framepicker-marblecanvas.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="default none" -->
![Workflow](../../assets/images/framepicker-capture.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/cameracapture-marble.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
![Workflow](../../assets/images/framepicker-grayscale.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/grayscalefile.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
![Workflow](../../assets/images/framepicker-grayscale.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/grayscaletransform.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
![Workflow](../../assets/images/framepicker-sample.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/grayscalesample.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
![Workflow](../../assets/images/framepicker-saveimage.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/saveimage.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
![Workflow](../../assets/images/framepicker-saveimage.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/saveimagesink.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
![Workflow](../../assets/images/framepicker-key.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/framepicker-marblecanvas.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
![Workflow](../../assets/images/framepicker.svg)
<!-- .element: style="display: inline-block; vertical-align: middle;" -->
![Marble diagram](../../assets/images/conditionkey.svg)
<!-- .element: class="fragment" style="display: inline-block; vertical-align: middle;" -->

---

##### Operator Categories

![Operator categories](../../assets/images/categories-simple.svg)
<!-- .element: style="padding: 30px; display: inline-block; vertical-align: middle;" -->

---

###### Skip

![Skip](../../assets/images/skip.svg)

---

###### Take

![Take](../../assets/images/take.svg)

---

###### SkipUntil

![SkipUntil](../../assets/images/skipuntil.svg)

---

###### TakeUntil

![TakeUntil](../../assets/images/takeuntil.svg)

---

###### Delay

![Delay](../../assets/images/delay.svg)

---

###### DelaySubscription / SubscribeWhen

![DelaySubscription](../../assets/images/delaysubscription.svg)

---

###### Repeat

![Delay](../../assets/images/repeat.svg)

---

###### Zip

![Zip](../../assets/images/zip.svg)

---

###### CombineLatest

![CombineLatest](../../assets/images/combinelatest.svg)

---

###### WithLatestFrom

![WithLatestFrom](../../assets/images/withlatestfrom.svg)

---

<!-- .element: data-transition="default none" -->
###### Transform

![Transform](../../assets/images/transform.svg)

--

<!-- .element: data-transition="default none" -->
###### Select

![Select](../../assets/images/select.svg)

--

<!-- .element: data-transition="none default" -->
###### SelectMany

![SelectMany](../../assets/images/selectmany.svg)

--

<!-- .element: data-transition="none default" -->
###### SelectMany: Play audio on cue

![SelectMany](../../assets/images/selectmany-playsound-1.svg)

--

<!-- .element: data-transition="none default" -->
###### SelectMany: Play audio on cue

![SelectMany](../../assets/images/selectmany-playsound-2.svg)

---

<!-- .element: data-transition="default none" -->
###### Buffer

![Buffer](../../assets/images/buffer.svg)

--

<!-- .element: data-transition="none default" -->
###### Buffer: Moving Average

![SelectMany](../../assets/images/buffer-movingaverage.svg)

---

<!-- .element: data-transition="default none" -->
###### TriggeredBuffer

![TriggeredBuffer](../../assets/images/triggeredbuffer.svg)

--

<!-- .element: data-transition="none default" -->
###### TriggeredBuffer: Signal Snapshot

![SelectMany](../../assets/images/triggeredbuffer-snapshot.svg)

---

###### Window

![Window](../../assets/images/window.svg)

---

<!-- .element: data-transition="default none" -->
###### TriggeredWindow

![TriggeredWindow](../../assets/images/triggeredwindow.svg)

--

<!-- .element: data-transition="none default" -->
###### TriggeredWindow: Record triggered video

![SelectMany](../../assets/images/triggeredwindow-recordclip.svg)

</script>
</section>

<section data-markdown data-separator="^\n---\n$" data-separator-vertical="^\n--\n$">
<script type="text/template">

![Bonsai](../../assets/images/bonsai-lettering.svg)

### Questions?
[neurogears.org/vrp-2022](https://neurogears.org/vrp-2022)
<table style="width: 100%;">
  <tr>
    <th style="vertical-align: middle; width: 50%; height: 100px; padding-left: 100px">
      <img alt="NeuroGEARS" src="../../assets/images/neurogears.svg"/>
    </th>
    <th style="vertical-align: middle; width: 50%; height: 100px; align: right">
      <img alt="Cajal" src="../../assets/images/cajal.png"/>
    </th>
  </tr>
</table>

</script>
</section>