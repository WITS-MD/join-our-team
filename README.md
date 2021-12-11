<img src="https://immd-public-logos.s3.us-east-2.amazonaws.com/immd-on-light.png" width="325">

ImageMover has an immediate opening for a software developer that will help build our suite of patient-focused 
healthcare products. This is a rare opportunity to join our passionate, highly-motivated team.

## What you'll do:

 * Write high-performance server code in Java and Node.
 * Craft user interfaces in HTML, CSS, Javascript and Typescript.
 * Design scalable, high-performance relational databases (MySQL) and document stores (MongoDB and DynamoDB).
 * Provide and receive constructive feedback during peer code reviews.
 * Collaborate with our customer success, quality assurance, product management and sales teams to ensure our 
   products release on time and delight our customers.

## You're the right cultural fit if you:

 * Demonstrate sensibility, flexibility, initiative and ownership.
 * Have the self-discipline required to contribute clean, simple and maintainable code.
 * Recognize that asking questions is a strength, not a weakness.
 * Love getting stuff done and having fun while doing it.

## About ImageMover

ImageMover is a healthy, fast-growing startup based in beautiful Madison, WI. We're remote friendly but if 
you're in the area, we also have a conveniently-located office near the University of Wisconsin.

* Flexible vacation policy encouraging a healthy work-life balance
* Strong insurance benefits package
* 401K with company matching
* Generous holiday schedule including Election day and Juneteenth
* Paid volunteer day each year
* Employee stock options

## How to Apply

Skip the boring cover letter. Complete the exciting programming challenge detailed below instead! The ideal candidate should be able to complete it in under 20 minutes.

Email your completed, functioning code (as a .zip file), your resume and a brief intro to [careers@imagemovermd.com](careers@imagemovermd.com).

## Programming Challenge

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

Refer to the [input](input.json?raw=true) and [output](output.json?raw=true) files for an example of what the method
will receive and produce.

In either [Java](UserUtils.java?raw=true) or [Node](UserUtils.js?raw=true), write the **simplest**, **cleanest** and
most **maintainable** code that meets the requirements identified above. Your submitted code can contain as many
additional methods as necessary to achieve this goal (e.g. you are not limited to a single function). The order of the
attributes in the returned object is irrelevant.

### Good luck!
