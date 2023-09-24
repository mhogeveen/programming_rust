# Mandelbrot

## `mandel_1.png`

Optimized release build, but no use of concurrence.

![mandel 1](./mandel_1.png)

### Command used

```sh
time mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
```

### `time` data

| resource | description |
| -------- | ----------- |
| 96%      | cpu         |
| 3.54s    | user        |
| 0.02s    | system      |
| 3.697    | total       |
