---
title: "Kayne's Error Handling, Documented"
categories: [technical]
tags: [code, emotional-intelligence]
excerpt: "A reverse-engineered look at how Kayne processes things going wrong."
---

We reverse engineered how Kayne handles errors. Here's our best reconstruction:

```python
def handle_problem(problem):
    try:
        stay_calm()
        make_a_list(problem)
        fix_top_item()
    except EverythingIsOnFire:
        stay_calm()          # yes, again
        ask_team_for_help()
        fix_top_item()
    finally:
        thank_everyone()
        write_documentation()
```

Notice there's no `panic()` call anywhere. We checked. It doesn't exist in the codebase.

Our version of this function is mostly `panic()`. We're working on it.
