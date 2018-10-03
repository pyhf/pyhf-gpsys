# Gaussian Process based interpolators for HistFactory (pyhf)

![Alt text](img/gpsys.png?raw=true "Title")


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
            "evals": [ #(sample bin, alphaval, delta)
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

