I deploy this onto out ovh k8s clusters, a deployment for each autoscaling nodepool, so that the created nodes will be retained for as long as possible.
This way if more work comes in during the time when the inital nodes were created, in that 1 hour window, they will get reused again. Instead of the nodes having scaled down, and now having to scale up new ones.
