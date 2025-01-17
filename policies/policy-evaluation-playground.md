# Policy Evaluation Playground

build.security provides some easy-to-use features that enable you to streamline the policy creation process while minimizing any impact this might have on your users. As you create your policies, you will want to evaluate the impact they have on your organization and then, depending on the outcome, consider adjusting some or all of the policy rules as needed.

{% hint style="info" %}
**Note**

The playground will use the PDPs running in your cluster in order to have access to the different data-sources, but will have _no effect_ on the deployed policies within those PDPs \(until explicitly published\).
{% endhint %}

The policy evaluation playground enables you to initiate a dry run authorization request to one of your PDPs to test the changes that you've made in the policy rule in real time, regardless of the policy status. This area, accessed by clicking the policy evaluation playground icon, will open on the right side of the policies screen. \(For more information, see [Dry Run Evaluation](https://docs.build.security/docs/dry-run-evaluation).\)

![Policy evaluation playground icon](https://files.readme.io/b234d69-polevaluicon.PNG)

After entering the code you wish to evaluate in the Input window, you can select the PDP that you'd like to use for this evaluation, and then click **EVALUATE**. The "_Use Cache_" checkbox specifies whether the data-source's cache option should be enabled for the evaluation attempt. For more information, see [Data Sources](https://docs.build.security/docs/data-sources-1) and review the data sources which support the caching option.

The policy evalutation playground can help reduce the time it takes you to author a policy by enabling you to "test-as-you-go." The evaluation calculation is performed with an active PDP instance, so before attempting to use this feature, you should first [verify](https://docs.build.security/docs/policy-decision-points) that you have an active PDP configured.

{% hint style="info" %}
**Note**

If you do not have an active PDP instance configured, see [Deploying a PDP](https://docs.build.security/docs/deploying-a-pdp).
{% endhint %}

![Policy evaluation playground](https://files.readme.io/5a581d4-policyevalplayground.png)



