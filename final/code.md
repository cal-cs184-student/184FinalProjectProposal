```python
f = init_fringe()
for r in radius_list:
    if f.empty():
        f = find_seed_triangle()
    if f is None:
        break
    for pivot_edge in f.edges():
        expand_triangle(pivot_edge)
```


