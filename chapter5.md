---
title: 'What is Bayesian Data Analysis?'
description: 'This chapter will introduce you to Bayesian data analysis and give you a feel for how it works.'
---

## Coin flips with prop_model

```yaml
type: TabExercise
key: 02b6a540f9
lang: r
xp: 100
skills: 1
```

The function `prop_model` has been loaded into your workspace. It implements a Bayesian model that assumes that:

 * The `data` is a vector of successes and failures represented by `1`s and `0`s.
 * There is an unknown underlying proportion of success.
 * Prior to being updated with data any underlying proportion of success is equally likely.

Assume you just flipped a coin four times and the result was *heads*, *tails*, *tails*, *heads*. If you code *heads* as a success and *tails* as a failure then the following R codes runs `prop_model` with this data
```{r}
data = c(1, 0, 0, 1)
prop_model(data)
```

`@instructions`


`@hint`


`@pre_exercise_code`
```{python}
eval(parse("http://s3.amazonaws.com/assets.datacamp.com/production/course_5334/datasets/beta_binomial_function.R"))
```

`@sample_code`
```{sql}

```

`@solution`
```{sql}

```

`@sct`
```{python}

```

`@possible_answers`


`@feedback`


***

```yaml
type: MultipleChoiceExercise
key: 99ab0345fc
xp: 100
```



`@instructions`


`@hint`
Look at the distribution at n=4. What value is it centered on? How wide is it spread out?

`@pre_exercise_code`
```{r}

```

`@sample_code`
```{r}

```

`@solution`
```{r}

```

`@sct`
```{r}
msg1 = "That's right! The model knows it's not close to 0% or close to 100%, but believes it could be anything in between."
msg2 = "Well, the model has a bit more information than that."
msg3 = "The probability distribution is symmetrical around 50% which means this is not the case."
msg4 = "If you look at the distribution at n=4 you see that it spans the range 5% to 95%."
test_mc(correct = 1, feedback_msgs = c(msg1,msg2,msg3, msg4))
```

`@possible_answers`
- It's most likely around 50%, but there is large uncertainty.
- It could be anywhere from 0% to 100%.
- It's more likely to be above 50%.
- It is close to 50% with high probability.

`@feedback`

---

## Insert exercise title here

```yaml
type: VideoExercise
key: c357294a7e
xp: 50
```

`@projector_key`
ff7647e84536d48ee3f7bac1e6b88325
