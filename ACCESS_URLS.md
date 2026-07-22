# LinkedIn Clone Public Access URLs

This file lists the current public demo endpoints for the EKS deployment.

## Application

Frontend:

```text
http://ade5840dc3ec0494cba966d84b187f2c-490133502.eu-west-2.elb.amazonaws.com:3000
```

API Gateway:

```text
http://ac2511ef9149847f0ae9ed56e0f05ba3-876930999.eu-west-2.elb.amazonaws.com:8085
```

Keycloak:

```text
http://a9099f2319da740c3b1c3e37813205aa-704837357.eu-west-2.elb.amazonaws.com:8080
```

## Observability

Grafana:

```text
http://a76e72fcac9fb4e6aa611943a8337b77-1324077080.eu-west-2.elb.amazonaws.com
```

Grafana login:

```text
Username: admin
Password: puX9btJPUPT5y45facsnBLyjikKne5hwyZP1q1SV
```

Prometheus:

```text
http://aeb63a034ee854aa6a30eb566648ad8a-815741197.eu-west-2.elb.amazonaws.com:9090
```

Recommended Grafana dashboard:

```text
LinkedIn Clone - Full Stack Observability
```

## CI/CD

Jenkins:

```text
http://af0c0b0ddc88741699248ca5be61c644-817734411.eu-west-2.elb.amazonaws.com:8080
```

Jenkins initial admin password:

```text
aea0229c64bb42fd920e93132f65a642
```

## Demo Notes

- Prometheus is currently public and does not have login protection.
- Jenkins is deployed with temporary `emptyDir` storage for the demo because EBS PVC provisioning was not working.
- For production, restrict these endpoints using VPN, private ingress, IP allowlists, authentication, or an ALB with HTTPS and access controls.
- After the presentation, remove or lock down public Prometheus and Jenkins access.

