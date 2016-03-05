
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
1. Run `jekyll new MyNewBlog`
2. Copy  **_source** and **build.R** into the directory created
3. type `cd MyNewBlog`
4. type `jekyll build`
5. type `R` , to open R in terminal.
6. type `servr::jekyll()`
 - if you get errors, install the required packages
7. Go to the address mentioned.


## How to add a new post:




 ## Credit:
THANK YOU Yihui, [Yijui's template](https://github.com/yihui/knitr-jekyll).
