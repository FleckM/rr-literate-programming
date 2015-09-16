# Literate Programming

## People

-  Jennifer Bryan: [@jennybc]
-  Hilmar Lapp: [@hlapp]
-  **Ciera Martinez** [@iamciera]
-  Kristina Riemer kristina.riemer@weecology.org
-  Courtney Soderberg courtney@cos.io
-  Naupaka Zimmerman: [@naupaka]

## Overview and learning objectives

Students will complete an activity highlighting the structure of
spreadsheet-type data files, emphasizing the importance of documenting
any changes made. They will then learn and apply a literate
programming approach to cleaning data files in the context of a
reproducible project workflow centered around using `knitr` in
RStudio.

At the begining of the session, students should

- be familiar with Rstudio: Rstudio layout, running R commands, knitr,
  and basic ggplot syntax (from Intro section)

At the end of the session students will be able to

- Distinguish between a spreadsheet formatted properly for later
  analysis in R and one formatted improperly
- Be able to recognize common data entry errors and how to handle them
- Be able to describe the concept of 'raw data' and why it is important
- Differentiate between manual and programmatic file manipulation and
  know the pros and cons of each

## Documenting data modifications

Lesson: [02-programatic-modification](02-documenting-data-modification.md)

### Activity 1 - Cleaning up data in Excel

In this section, the students will explore why it is beneficial to do
programmatic modification by exploring what it takes to clean up a
data file in Excel.

## Literate programming - R via RStudio 

* Lesson: [03-literate-programming](03-literate-programming.md)
* [Introductory slides](slides/lit-prog-slides)

### Activity 

**Note: could overlap in part with Intro, Activity 2; may require
  on-the-fly adjustments in response to that.**

Students "knit" and modify. Using
[countryPick4.Rmd](files/lit-prog/countryPick4.Rmd) as a template,
students learn how to import data, filter to one country, make a plot,
write it to file, and comment data choices.  Then the activity will
illustrate what happens when you knit:
- Preview/Knit HTML, note what sorts of outputs are left behind.
- Discuss input and output files.
- Which files can we delete and reproduce? Which files are inputs,
  outputs, converters of inputs to outputs?

This section is meant for students to explore the power of writing
reports in R.


## Resources and useful links

### Relevant scientific papers

- EP White, E Baldridge, ZT Brym, KJ Locey, DJ McGlinn, SR
  Supp (2013) "Nine simple ways to make it easier to (re)use your
  data." Ideas in Ecology and Evolution 6(2):
  1–10, 2013. doi:[10.4033/iee.2013.6b.6.f] _(in particular the
  section "Use standard table formats")_
- WS Noble (2009) "A Quick Guide to Organizing
  Computational Biology Projects." PLoS Computational Biology 5 (7):
  e1000424. doi:[10.1371/journal.pcbi.1000424]

### Best practices for spreadsheets

- [Good practice guidance on releasing statistics in spreadsheets](UK Government)

## License and Attribution

- [Gapminder data](http://www.gapminder.org/data/). [Gapminder data is licensed CC-BY 3.0](https://docs.google.com/document/pub?id=1POd-pBMc5vDXAmxrpGjPLaCSDSWuxX6FLQgq5DhlUhM#h.ul2gu2-uwathz).
- Processed and subset (population size, life expectancy, GDP per
  capita; only every 5 years only starting 1952, only complete records)
  [Gapminder data as R package](https://github.com/jennybc/gapminder). The [data-raw](https://github.com/jennybc/gapminder/tree/master/data-raw) sub-directory reveals the journey from Gapminder.org's Excel workbooks to increasingly clean and tidy data.
    - clean dataset can be located in R in the following way (after
      installing the package):

        ```R
        pathToTsv <- system.file("gapminder.tsv", package = "gapminder")
        ```

- All other lesson material is dedicated to the public domain under
  the [CC Zero] waiver.


[@jennybc]: http://github.com/jennybc
[@hlapp]: http://github.com/hlapp
[@iamciera]: http://github.com/iamciera
[File Naming Conventions & Best Practices]: http://researchdata.library.ubc.ca/organize
[File Format Considerations]: http://researchdata.library.ubc.ca/format/
[List of filename extensions]: http://en.wikipedia.org/wiki/List_of_file_formats
[ISO 8601 standard for dates]: http://en.wikipedia.org/wiki/ISO_8601
[Good practice guidance on releasing statistics in spreadsheets]: https://gss.civilservice.gov.uk/wp-content/uploads/2012/12/Releasing-statistics-in-spreadsheets-Good-practice-guidance.pdf
[10.4033/iee.2013.6b.6.f]: http://dx.doi.org/10.4033/iee.2013.6b.6.f
[10.1371/journal.pcbi.1000424]: http://dx.doi.org/10.1371/journal.pcbi.1000424
[CC Zero]: https://creativecommons.org/publicdomain/zero/1.0/
