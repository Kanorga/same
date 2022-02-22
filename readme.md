# Node Types:
## **Navigation Panel**
* [Service](#service:)
* [Action](#action:)
* [Publisher](#publisher:)
![Markdown Logo] (${{ github.workspace }}/happy-person-11545688398rslqmyfw4g.png)

## **Service:** 
#### **Summary:**
Async, no progress, single "one-shot" with "finished" feedback. 

#### **Examples:**
* GPU: color this final image *(from 2 image inputs)*. 
  * Client calls color_image *(im1, im2, etc)*
  * GPU processes coloring, then finishes *(In its QoS queue)*
  * Depending on blocking or async, client blocks or does callback
#### Notes:
* Service makes sense when it's managing a limited resource. 
  * Examples: GPU, shared 	memory, devices
* Server queues up stuff per node *(managed by QoS)*


## <a name ="Action"></a> **Action:** 

