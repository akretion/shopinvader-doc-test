---
# Given `ordered` is set to true, an ordered list should be output instead of an unordered list
---

{% capture markdown %}
# Heading 1

## Heading 2.1

### Heading 3

#### Heading 4

## Heading 2.2
{% endcapture %}
{% assign text = markdown | markdownify %}

{% include toc.html html=text ordered=true %}

