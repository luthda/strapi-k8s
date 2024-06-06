# FoodAdvisor - Kubernetes Deployment

This project includes a demo application, FoodAdvisor, which connects to a Strapi CMS as the backend API. The entire application is deployed on Kubernetes.

Link FoodAdvisor repo: <https://github.com/strapi/foodadvisor>

## Architecture

The application consists of two main components:

1. **FoodAdvisor Client**: This is the front-end of the application where users can interact with the system.

2. **Strapi CMS**: This is the backend API that serves data to the FoodAdvisor client. It uses a PostgreSQL database to store its data.

Both components are deployed on a Kubernetes cluster. An Ingress is set up to manage incoming traffic, directing it to the appropriate services.

## Deployment

The Kubernetes manifests for the deployments, services, and ingress can be found in the `k8s` directory. Please contact me for api keys for strapi. To deploy the application, navigate to this directory and apply the manifests:

```bash
kubectl apply -f .
```

Ensure that you have a running Kubernetes cluster and that kubectl is configured to interact with it.

Accessing the Application
Once deployed, the application can be accessed through the URL specified in the Ingress configuration.

Contributing
Contributions are welcome! Please read the contributing guidelines before making any changes.

License
This project is licensed under the MIT License - see the LICENSE.md file for details.
