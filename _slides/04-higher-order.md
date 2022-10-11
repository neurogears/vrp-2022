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

---

###### Amb

![Amb](../../assets/images/amb.svg)

---

###### Merge

![Merge](../../assets/images/merge.svg)

---

###### Concat

![Concat](../../assets/images/concat.svg)

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