---
layout: slides
title: Higher Order Operators
permalink: /slides/higher-order/
---

<section data-markdown data-separator="^\n---\n$" data-separator-vertical="^\n--\n$">
<script type="text/template">

![Bonsai](../../assets/images/bonsai-lettering.svg)

### Higher Order Operators
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
* Sharing Sequences
* Higher Order Operators

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

### Sharing observable sequences

![Branching](../../assets/images/branching-simple.svg)
<!-- .element: style="display: inline-block; vertical-align: top;" -->
![Subjects (Publish)](../../assets/images/subjects-publish-simple.svg)
<!-- .element: class="fragment" style="display: inline-block; vertical-align: top; padding-left: 120px;" -->

--

### Sharing observable sequences

![Publish](../../assets/images/publish.svg)
<!-- .element: style="display: inline-block; vertical-align: top;" -->
![Replay](../../assets/images/replay.svg)
<!-- .element: class="fragment" style="display: inline-block; vertical-align: top; padding-left: 40px;" -->

--

### Sharing observable sequences

![Subjects (Publish)](../../assets/images/subjects-publish.svg)
<!-- .element: style="display: inline-block; vertical-align: top; padding-left: 120px;" -->
![Subjects (Replay)](../../assets/images/subjects-replay.svg)
<!-- .element: class="fragment" style="display: inline-block; vertical-align: top; padding-left: 120px;" -->

---

<!-- .element: data-transition="default none" -->
### Subject Types

![Subject types](../../assets/images/subjects-declaration.svg)
<!-- .element: style="padding: 30px; display: inline-block; vertical-align: middle;" -->

--

<!-- .element: data-transition="none" -->
### Subject Types

![Subject types](../../assets/images/subjects.svg)
<!-- .element: style="padding: 30px; display: inline-block; vertical-align: middle;" -->

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
###### BufferTrigger

![BufferTrigger](../../assets/images/buffertrigger.svg)

--

<!-- .element: data-transition="none default" -->
###### BufferTrigger: Signal Snapshot

![BufferTrigger](../../assets/images/buffertrigger-snapshot.svg)

---

###### Window

![Window](../../assets/images/window.svg)

---

<!-- .element: data-transition="default none" -->
###### WindowTrigger

![WindowTrigger](../../assets/images/windowtrigger.svg)

--

<!-- .element: data-transition="none default" -->
###### WindowTrigger: Record triggered video

![WindowTrigger](../../assets/images/windowtrigger-recordclip.svg)

---

###### Merge

![Merge](../../assets/images/merge.svg)

---

###### Concat

![Concat](../../assets/images/concat.svg)

---

### Higher-Order Operators

![Concatenate video files using first order operators](../../assets/images/concatfile-firstorder.svg)

--

###### Enumerate Files

![Enumerate all file names in a folder](../../assets/images/concatfile-enumeratefiles.svg)

--

###### Create Observable

![Create sequences of frames from file names](../../assets/images/concatfile-observable.svg)

--

###### Concat

![Combine all sequences of frames into a single sequence](../../assets/images/concatfile-combine.svg)

--

###### Higher-Order: Batch concatenate multiple videos

![SelectMany](../../assets/images/higherorder-concatfiles.svg)

---

###### Concat

![Concat](../../assets/images/concatwindow.svg)

---

###### Merge

![Merge](../../assets/images/mergewindow.svg)

---

###### Switch

![Switch](../../assets/images/switch.svg)

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