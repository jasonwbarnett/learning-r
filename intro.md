Intro to R
==========

- Assignment operator: `<-`
- Assign variable: `mynum <- 44`
- List all defined variables in workspace: `ls()`

#### Sample R script:

    # rectangle.R
    height <- 2
    width <- 4
    area <- height * width
    area

- Remove variable from workspace: `rm(area)`
- Determine type of value/variable: `class(<value>)`
  - e.g. `class(TRUE)`

### R Data types aka atomic vector types

#### logical

- `TRUE`, `T`
- `FALSE`, `F`
- `NA`

#### numeric

- `2`
- `2L`
- `class(2)` vs `class(2L)`
- `2.5` is numeric

        > is.numeric(2)
        [1] TRUE
        > is.numeric(2L)
        [1] TRUE
        > is.integer(2)
        [1] FALSE
        > is.integer(2L)
        [1] TRUE

integer __is__ numeric
numeric __not always__ integer

#### character

    > "I love my life."
    [1] "I love my life."
    > class("I love my life.")
    [1] "character"

#### other atomic types

- double: higher precision
- complex: complex numbers
- raw: store raw bytes
