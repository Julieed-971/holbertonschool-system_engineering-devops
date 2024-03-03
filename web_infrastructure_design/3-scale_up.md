## For every additional element, why are you adding it:

The final added component is another HAProxy configured as cluster with the other one.
This resolve the remaining single point of failure.
Components are separated in different servers in order to avoid failure to one component to spread to the others.