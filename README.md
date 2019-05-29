# Kubernetes car for the [Bullettrain](https://github.com/bullettrain-sh/bullettrain-go-core) shell prompt

## Features:

- Displaying only when kubectl installed
- Kubernetes context display


**Callword**: `k8s`

**Template variables**:

* `.Icon`: the car's icon
* `.Context`: the Kubernetes context text

**Template colours**:

* `c`: the car's colour


## Car options

| Environment variable                  | Description                                                    | Default value                                   |
|:--------------------------------------|:---------------------------------------------------------------|:------------------------------------------------|
| BULLETTRAIN_CAR_K8S_SHOW               | Whether the car needs to be shown all the time.                | true                                           |
| BULLETTRAIN_CAR_K8S_TEMPLATE           | The car's template.                                            | `{{.Icon \| printf " %s " \| c}}{{.Context \| c}}` |
| BULLETTRAIN_CAR_K8S_PAINT              | Colour override for the car's paint.                           | white+h:yellow                                       |
| BULLETTRAIN_CAR_K8S_SYMBOL_ICON        | Icon displayed on the car.                                     | `⎈`                                             |
| BULLETTRAIN_CAR_K8S_SEPARATOR_PAINT    | Colour override for the car's right hand side separator paint. | Using default painting algorythm.               |
| BULLETTRAIN_CAR_K8S_SEPARATOR_SYMBOL   | Override the car's right hand side separator symbol.           | Using global symbol.                            |
| BULLETTRAIN_CAR_K8S_SEPARATOR_TEMPLATE | Defines the car separator's template.                          | Using global template.                          |

# Contribute

Even reporting your use case will greatly help us to figure out/improve
this product, so feel free to reach out in the Issues section.
