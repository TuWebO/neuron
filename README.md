# neuron
Reports out of google sheet conected and related data.

## Brain
Google sheet containing the data. All other sheets will show data out of this one. Is the only sheet that should be edited.

E.g.: A folder estructure.
- foo/bar/one.txt
- two.txt

## Neurons
Google sheet normalized data. Uses Brain Data.

E.g.: Complete folder estructure (applying some rules, if any). 
- foo/bar
- foo/bar/one.txt
- two.txt

## Connections
Google sheet data representing connections between Neurons. 
Neurons with no Connections are considered the brain.
They should be using Relations so everybody knows what is going on between Neurons.

E.g.: **foo/bar** and **foo/bar/one.txt** have conections. **two.txt** has no conexion.
- foo/
- foo/bar/
- 

## Relations
Represents the connection and it meaning.

E.g.: In the above example a regexp like ```.+\/**``` could be called Parent relation and actually should the one being used for generating the Connections.


## Dashboard
Contains as many sheets as necesary for representing the data. Could be used for Charts visualization.
