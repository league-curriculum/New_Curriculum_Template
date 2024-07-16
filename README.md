# New Curriculum Template

Template for vuepress-based lesson websites. 

NOTE! This is a template site, so use the template, don't clone it. 


## Using this Repo


### Install the lesson builder program and vuepress

To install the lesson builder, first [install pipx](https://pipx.pypa.io/latest/installation/) then install
`lesson-builder` with pipx:

```bash
pipx install git+https://github.com/league-infrastructure/lesson-builder.git
```

Install vuepress, if you haven't already.  [See these instructions for details](https://vuepress.vuejs.org/guide/getting-started.html). 
in this example, we will be using `yarn` rather than `npm` to install vuepress.

If you have installed yarn previously, you will still need to install in the docs dir

```bash
 (cd docs &&  yarn install )
 ```


### Build the  Website source

Now you can build your website. 

```bash 
$ jtl -vv build -l lessons -w
INFO:lesson_builder.cli.jtl:Using url base 'LevelX'
INFO:lesson_builder.lesson:Writing lesson plan to docs/src/lessons
DEBUG:lesson_builder.lesson:Writing Lesson Introduction to Tina the Turtle to docs/src/lessons/introduction-to-tina-the-turtle
DEBUG:lesson_builder.lesson:        Copying flag.png to docs/src/lessons/introduction-to-tina-the-turtle
DEBUG:lesson_builder.lesson:        Writing Shapes and Colors
```

### Serve the website. 

```bash
jtl serve
```

If you get errors, it maybe because you need to install packages with yarn. Try: `(cd docs &&  yarn install )`

If it works, visit  http://localhost:8080/LevelX/ to see you site. 








