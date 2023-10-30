<img src="https://immd-public-logos.s3.us-east-2.amazonaws.com/immd-on-light.png" width="325">

ImageMover has an immediate opening for an entry-level software developer that will help build our suite of 
patient-focused healthcare products. This is a rare opportunity to join our passionate, highly-motivated team.

We’re looking for a skilled and motivated junior software engineer to join our team. Our ideal candidate will 
have knowledge of software development processes and experience developing client-side software. Software 
development includes IOS development, Android development, web development, and a significant fraction of time 
developing customer workflows on all of these platforms using our proprietary workflow engine. If learning new 
technologies and developing beautiful, meticulous code are among the talents that make you tick, we’d like to 
hear from you.

## What you'll do:

In this role, you will be a key member of the Software Development team reporting to the [SVP of Engineering](https://github.com/Thaliant). 
Your core responsibility will be to develop products that delight our customers as they deliver point of care 
services to their patients. 

Though we are looking for some specific skills – as noted in the list below – who you are is more important to 
us than what you know.  Attitude, values and raw talent are as important as specific experience.  Non-negotiable 
competencies include openness, team approach, and a strong focus on quality.  It is not necessary to have prior 
experience in healthcare or a deep knowledge of point of care testing.  You will gain extensive knowledge in 
both areas on the job.

 * Develop customer workflows on IOS, Android, and Web.
 * Craft user interfaces in HTML, CSS, Javascript.
 * Enhance our mobile applications in Swift and Kotlin.
 * Provide and receive constructive feedback during peer code reviews.
 * Collaborate with our customer success, quality assurance, product management and sales teams to ensure our
   products release on time and delight our customers.
 * Support and comply with the company’s Quality Management System policies and procedures.

## You're the right cultural fit if you:

 * Have excellent problem-solving and communication skills
 * Are a self-starter
 * Have the ability to resolve issues timely and accurately
 * Have effective time management to include establishing priorities and meeting deadlines
 * Exhibit continuous improvement skills to make processes more efficient
 * Are detail oriented
 * Uphold the company mission and values through accountability, innovation, integrity, quality, and teamwork
 * Have the bility to work in fast-paced environment with demonstrated ability to manage multiple competing priorities

## About ImageMover

ImageMover is a healthy, fast-growing startup based in beautiful Madison, WI. We're remote friendly but if 
you're in the area, we also have a conveniently-located office near the University of Wisconsin.

With our [Workflow Services](https://www.workflowservices.com/) platform, we’re helping to drive the evolution of medical care delivery in retail 
and community pharmacies.  Our platform allows for rapid iteration of digital workflows to support the specific 
needs of a customer.  This team member has the opportunity to support our growth as we add new customers and 
drive evolution of the system as we always look for more scalability and efficiency.

* Flexible vacation policy encouraging a healthy work-life balance
* Strong insurance benefits package
* 401K with company matching
* Generous holiday schedule including Election day and Juneteenth
* Paid volunteer day each year
* Employee stock options

## How to Apply

Skip the boring cover letter. Complete the exciting programming challenge below *instead!* The ideal candidate should 
be able to complete it in under 20 minutes.

Email your completed, functioning code (as a .zip file), your resume and a brief intro to 
[careers@imagemovermd.com](careers@imagemovermd.com). Having trouble getting it to us? Send us an email and we’ll give 
you a secure link to upload everything. 

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
