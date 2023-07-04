# protopackage

An empty R package build as a prototype. It illustrates development practices in R: documentation, literate programming, testing, versioning, continuous integration.

  
**Install**
  
```
devtools::install_github("fchuffar/protopackage")
```
  
  
**Developement**

On a terminal:

```
git clone git@github.com:fchuffar/protopackage.git
cd protopackage
```

Under R:
    
```
devtools::document(); 
devtools::install(); 
Sys.setenv('_R_CHECK_SYSTEM_CLOCK_' = 0)
devtools::check()
devtools::build()
```

**Vignettes**


Under R, in the vignette directory:
    
```
rmarkdown::render("make_a_coffee.Rmd")
```
