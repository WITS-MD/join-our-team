# Programming Challenge

After authentication, AWS Cognito returns a JSON user object in a suboptimal, nested format with attributes that don't
adhere to our variable naming conventions.

You are tasked with writing a method that, when passed a Cognito JSON object, returns a flattened object with more
consistent attribute names, thereby making it easier for other parts of our software to work with user instances in an
API agnostic way.

1. User objects will always have a `UserAttributes` array. It will always include `sub` and `email` entries. All other
   attributes are optional. Not all attributes are present in the example file.
2. Returned attribute names must be in TitleCase.
3. Prefixes (e.g. `custom`) should be removed. Prefixes will always be delimited by a colon.
4. Boolean attributes should be returned as booleans, rather than strings.
5. If the user has `custom:tags`, they are stored as a comma-delimited string. The returned object should return an
   array of tags so callers don't have to do string manipulation themselves.
6. Do not include the `sub` attribute in the returned object because, like code, data should also be DRY.
7. The returned object must include a `DisplayName` attribute. This should be `"Family, Given"`, their given name or
   their email address, depending on what is available.

Refer to the [input](input.json) and [output](output.json) files for an example of what the method will receive and
produce.

In either [Java](UserUtils.java) or [Node](UserUtils.js), write the **simplest**, **cleanest** and most **maintainable**
code that meets the requirements identified above. Your submitted code can contain as many additional methods as
necessary to achieve this goal (e.g. you are not limited to a single function). The order of the attributes in the
returned object is irrelevant.
