# AWS::CodeCommit::Repository RepositoryTrigger<a name="aws-properties-codecommit-repository-repositorytrigger"></a>

Information about a trigger for a repository\.

## Syntax<a name="aws-properties-codecommit-repository-repositorytrigger-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-codecommit-repository-repositorytrigger-syntax.json"></a>

```
{
  "[Branches](#cfn-codecommit-repository-repositorytrigger-branches)" : [ String, ... ],
  "[CustomData](#cfn-codecommit-repository-repositorytrigger-customdata)" : String,
  "[DestinationArn](#cfn-codecommit-repository-repositorytrigger-destinationarn)" : String,
  "[Events](#cfn-codecommit-repository-repositorytrigger-events)" : [ String, ... ],
  "[Name](#cfn-codecommit-repository-repositorytrigger-name)" : String
}
```

### YAML<a name="aws-properties-codecommit-repository-repositorytrigger-syntax.yaml"></a>

```
  [Branches](#cfn-codecommit-repository-repositorytrigger-branches): 
    - String
  [CustomData](#cfn-codecommit-repository-repositorytrigger-customdata): String
  [DestinationArn](#cfn-codecommit-repository-repositorytrigger-destinationarn): String
  [Events](#cfn-codecommit-repository-repositorytrigger-events): 
    - String
  [Name](#cfn-codecommit-repository-repositorytrigger-name): String
```

## Properties<a name="aws-properties-codecommit-repository-repositorytrigger-properties"></a>

`Branches`  <a name="cfn-codecommit-repository-repositorytrigger-branches"></a>
The branches that will be included in the trigger configuration\. If you specify an empty array, the trigger will apply to all branches\.  
Although no content is required in the array, you must include the array itself\.
*Required*: No  
*Type*: List of String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`CustomData`  <a name="cfn-codecommit-repository-repositorytrigger-customdata"></a>
Any custom data associated with the trigger that will be included in the information sent to the target of the trigger\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`DestinationArn`  <a name="cfn-codecommit-repository-repositorytrigger-destinationarn"></a>
The ARN of the resource that is the target for a trigger\. For example, the ARN of a topic in Amazon SNS\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Events`  <a name="cfn-codecommit-repository-repositorytrigger-events"></a>
The repository events that will cause the trigger to run actions in another service, such as sending a notification through Amazon SNS\.   
The valid value "all" cannot be used with any other values\.
*Required*: No  
*Type*: List of String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Name`  <a name="cfn-codecommit-repository-repositorytrigger-name"></a>
The name of the trigger\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)