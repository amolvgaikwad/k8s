# kubernetes-templates

# Service 

An abstract way to expose an application running on a set of Pods as a network service.
With Kubernetes you don't need to modify your application to use an unfamiliar service discovery mechanism. Kubernetes gives Pods their own IP addresses and a single DNS name for a set of Pods, and can load-balance across them.


Kubernetes Pods are created and destroyed to match the state of your cluster. Pods are nonpermanent resources. If you use a Deployment to run your app, it can create and destroy Pods dynamically.

Kubernetes Pods are created and destroyed to match the desirable state of your cluster. Each pod got its own unique ip address.  

Consider if set of backend pods and set of front end pods running in the same cluster, Obiiously front end pods needs to access backend pods but due to nonpermanent ip addess its impossible to keep track of those connection. So how frontend pods can keep reliable connection with backend pods? Here services will help you, with service component you can provide cluster level dns name to set of pods. 

lets discuss about services.