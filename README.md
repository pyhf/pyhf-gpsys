# Gaussian Process based interpolators for HistFactory (pyhf)

![Alt text](img/gpsys.png?raw=true "Title")


evaluations provided as (sample bin, ) + alpha-vector + (delta, )

```json
samplespec = {
    "name": "hello",
    "data": [0,0,0,0,0,0],
    "modifiers": [
        {
        "name": "mygp",
        "type": "gpsys",
        "data": {
            "kernel": "rbf_constant",
            "evals": [
                 [ 3, 0.5,-1.0, 15.0],
                 [ 5,-0.2, 0.8, 10.0],
                 [ 0,-1.0,-0.2, 20.0],
                 [ 5, 0.4, 0.9, 17.0],
                ]
            }
        }
    ]
}
```

