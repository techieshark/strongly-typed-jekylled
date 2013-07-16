---
layout: post
title:  "Welcome to Jekyll!"
date:   2013-07-13 00:01:57
categories: jekyll update
excerpt: "An introduction to the Jekyll system."
---

You'll find this post in your `_posts` directory - edit this post and re-build (or run with the `-w` switch) to see your changes!
To add new posts, simply add a file in the `_posts` directory that follows the convention: YYYY-MM-DD-name-of-post.ext.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll's GitHub repo][jekyll-gh].

Notes & Modifications:
<ul class="style1">
<li>Removed left sidebar, right sidebar, no-sidebar links from header wrapper (in \_includes/head-wrapper.html).  Rather than locating those files in the root directory, they're now layouts in \_layouts directory).  The default layout is used for the front page index (\_layouts/default.html), posts use the right hand sidebar layout (\_layouts/right-sidebar.html), and the strongly-typed.html and archive.html pages use the no-sidebar layout (\_layouts/no-sidebar.html). If you want a left sidebar, overwrite the post.html file with the contents of left-sidebar.html.</li>
<li>The site name and description shown at the top of pages is set in \_config.yml.</li>
<li>The contact info at the bottom of pages is set in \_config.yml.</li>
<li>Some lorum ipsum text from Stronly Typed has been replaced with text from [Space Ipsum](http://spaceipsum.com).</li>
<li>Strongly Typed's images have been replaced with images from placekitten / placedog etc (placeholder images of cats and dogs). The original images are still in the images/ directory.</li>
<li>The contact form doesn't yet work.</li>
<li>See the discussion of baseurl here: http://jekyllrb.com/docs/github-pages/.  You'll need to run jekyll with the --baseurl '' option if you're doing local development, and set baseurl appropriately in your _config.yml file.
</li>
</ul>

[jekyll-gh]: https://github.com/mojombo/jekyll
[jekyll]:    http://jekyllrb.com
