---
layout: post
title:  "Bits to Bytes in javascript"
date:   2025-02-20 11:48:32 +0100
categories: jekyll update
---

# Bits to Bytes

Today's task was to write a simple converter in Javascript that converts bits to bytes. I do not know what was ment by this exactly, so what i ended up making was a converter that converts a binary value to its hexadecimal representation.

The main task for me was figuring out how to link the button to getting the value of the input field. I eventually made this work by using the following code:

{% highlight html javascript %}
  <input type="text" placeholder="Bits here!">
  <button type="button" onclick="get_bin_input()">Convert!</button>


  <script>
  function get_bin_input() {
    InputBinary = document.getElementById("BinaryInput").value;
    alert(convert_to_hexa(InputBinary));
  }
  </script>

{% endhighlight %}

The converting to hexadecimal really wasn't that hard. The following code was all i needed, along with wrapping it in a function:

{% highlight javascript %}
function convert_to_hexa(binary) {
  var hexa = parseInt(binary, 2).toString(16);
  return hexa;
}
{% endhighlight %}

I've put it in a github repo as well, which you can check out [here](https://github.com/joploljojo3/bits_bytes_calc)!
