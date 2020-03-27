# 10converters Calculators

## Background

Calculating your grade is a skill which need just a little math. But it's always convenience to have a
handy tool to do it for you.

[10converts](https://10converters.com) provides a comprehensive set of grade calculators for college or
high school students and teachers.

* [grade calculator](https://10converters.com/calculators/grade-calculator), which calculate your current grade of a course
* [final grade calculator](https://10converters.com/calculators/final-grade-calculator), let you know what you should get in final exam to meet your desired overall class grade
* [semester grade calculator](https://10converters.com/calculators/semester-grade-calculator), calculates your overall grade in semeter or bimester
* [high school GPA calculator](https://10converters.com/calculators/high-school-gpa-calculator), GPA calculator for high school students and teachers
* [college GPA calculator](https://10converters.com/calculators/college-gpa-calculator), GPA calculator for college students and teachers

These tools are all implemented in Rust.

## Input

whatever the calculator you selected, a CSV file will always be the format of input.
```
Quiz, 90, 20
Homework, 85, 20
Midterm, 92, 30
```
That means you have your current grades of a specified course, e.g. History, and you want to know current
grade by far.

The first column is assessement name, but it's optional. you could write the CSV like:
```
Quiz, 90, 20
85, 20
92,30
```

The second column is grade, could be in percentage or in letters or in points:
```
Quiz, A, 20
Homewor, A-, 20
Midterm, A+, 30
```

## Output

each calculator module has it's own output. In general, it's a result in string like:

```
Your current grade is 91%(A)
```

like that. for different calculator, the output string is slightly different.