
# ExtensionsV1beta1IngressSpec

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**backend** | [**ExtensionsV1beta1IngressBackend**](ExtensionsV1beta1IngressBackend.md) | A default backend capable of servicing requests that don&#39;t match any rule. At least one of &#39;backend&#39; or &#39;rules&#39; must be specified. This field is optional to allow the loadbalancer controller or defaulting logic to specify a global default. |  [optional]
**rules** | [**List&lt;ExtensionsV1beta1IngressRule&gt;**](ExtensionsV1beta1IngressRule.md) | A list of host rules used to configure the Ingress. If unspecified, or no rule matches, all traffic is sent to the default backend. |  [optional]
**tls** | [**List&lt;ExtensionsV1beta1IngressTLS&gt;**](ExtensionsV1beta1IngressTLS.md) | TLS configuration. Currently the Ingress only supports a single TLS port, 443. If multiple members of this list specify different hosts, they will be multiplexed on the same port according to the hostname specified through the SNI TLS extension, if the ingress controller fulfilling the ingress supports SNI. |  [optional]



