
## Using R code in your blog
## AKA Making Jekyll work with knitr

### How to use these files

This contains the files you need to make a Jekyll blog run R code.
You need [Jekyll](http://jekyllrb.com) (hint: `gem install jekyll`)

You need R, and some packages:

- *servr* (>= 0.2)
- *knitr* (>= 1.8).
      - In R type `install.packages(c('servr', 'knitr'), repos = 'http://cran.rstudio.com')`


#### Basic use
1. Type into your terminal: `jekyll new MyNewBlog`
  - This sets up a folder containing all the files needed for a blog, written in _markdown_. Radical.
  - _Tip: Check this works without R by typing:_
    - `cd MyNewBlog`
    - `jekyll serve`
    - Check the webpage generated, it should be nicely styled. Cool? OK, let's do this.
2. Copy the files from this repo (**_source** and **build.R**) into the __MyNewBlog__ directory created
3. Navigate to this folder (Type into terminal: `cd MyNewBlog`, if you didn't already).
4. Type into terminal: `R`
  - This opens R in the terminal.
5. Type into terminal: `servr::jekyll()`
  - This runs the code which will turn **.Rmd** files in *_source_* to **.md** files in *_posts*.
  - Go to the address mentioned in the output to see the webpage, hosted locally.


## How to add a new .Rmd post:

1. Make a new file in **_source** called **year-month-day-Title.Rmd**
2. Copy contents of the included Post Template into the new, blank file
3. Replace title, date, etc (i.e. categories and tags)

## Maths

I'll talk later (or somewhere else) about adding maths (i.e. greek letters and formulas).

Hint: add this to *_config.yml*: `mathjax: true`, and add this to files in *_layouts* (not sure which ones, all works for me...)

```` html
<script type="text/javascript"
  src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
````


## Credit:

THANK YOU Yihui, [Yijui's template](https://github.com/yihui/knitr-jekyll).
