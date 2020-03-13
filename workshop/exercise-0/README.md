# Exercise 0 - Connect to Kubernetes cluster

Complete steps in this section to connect to your Kubernetes cluster.

1. Open a terminal window or command window.

    > **Note: use a web terminal if you attend a workshop**

1. Set an environment variable

    ```
    export USERNAME=user###
    ```

    > **Note: replace ### with your assigned ID**

1. Login to [Kubernetes service in IBM Cloud](https://cloud.ibm.com/kubernetes/clusters).

1. Select your Kubernetes cluster.

1. Navigate to `Access` tab.

    ![access-cluster](../README_images/access-cluster.png)

1. The section `After your cluster provisions, gain access` on your Kubernetes cluster window, provides commands to login to your IBM Cloud account and connect to your IKS cluster.

1. In the above terminal window, complete all steps in the section `After your cluster provisions, gain access`, including

    - Log in to your IBM Cloud account. Include the --sso option if using a federated ID.
    - Download the kubeconfig files for your cluster.
    - Set the KUBECONFIG environment variable.

    > Note: Don't forget to `Step 3. Set the KUBECONFIG environment variable.` Otherwise, you won't connect to your Kubernetes cluster.

1. Verify the connection to IBM Cloud and IKS cluster.

    ```
    ibmcloud target
    ```

    ```
    kubectl config view
    ```


#### [Continue to Exercise 3 - Deploy the Guestbook app with Istio Proxy](../exercise-3/README.md)

> Note: Exercise 1 and Exercise 2 are completed for a instructor-led workshop. If you are doing these exercises outside a workshop environment, you should complete `Exercise 1` and `Exercise 2` before moving onto `Exercise 3`.


