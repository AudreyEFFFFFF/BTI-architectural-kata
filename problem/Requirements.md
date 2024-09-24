# Business requirements

- The platform must parse candidate resumes into S.M.A.R.T. (Specific, measurable, achievable, relevant, time-bound) goal format to quantifiably match their skills and experience to job descriptions.
- The platform must provide a match score between roles and candidates.
- The platform AI must give job-seekers resume feedback and advice.
- The platform AI must remove any personal, racial, cultural, and lifestyle indicators.
- The platform must collect and aggregate data on hiring processes.

## For employers/companies
- Platform must provide ability to register for a company account
- Platform AI must automatically fill publicly-available company information into a company profile (user may add non-public-facing info via manual data entry)
- Platform must accept job descriptions for open roles as uploads
- Platform must find matching job candidate profiles and make them available to the user with match scores
- Platform must collect data on candidate demographic at various points moving forward through the hiring process (deciding to move forward with a candidate initially, unlocking a candidates full profile to offer an interview, and final offer/rejection)
- Platform must collect and store feedback on candidates/interviews
- User experience should be a dashboard and workspace

## For job candidates
- User must be able to register for an account
- User must be able to upload resume and supply additional information (ie contact, demographic)
- Platform must automatically parse resume information (user should not need to enter data twice)
- Platform AI must provide specific and personalized resume feedback and advice
- User must be able to update resume and other information
- User must be able to delete resume and other information
- User should be marked as inactive when hired
- Platform must collect and store user feedback on interviews
- User experience is not specified

## For platform administrators(/consultants?)
- User must be able to mark candidates as hired/jobs as filled
- User must have access to internal reference and user data
- User must have access to reporting and analytics
- User must have insight into and a way to provide feedback on job processes

## Other
- Platform must interface with popular HR software
- Platform will use an existing, pre-trained LLM for this purpose


# Technical requirements
- Secure data storage for user information/accounts (companies/candidates/administrators)
- Collection and storage of analytic data (anonymized demongraphic data on candidates, 	deciding to move forward with a candidate, unlocking a full candidate profile to offer an interview, 5 question survey to job candidate about interviewer, 5 question survey to interviewer about job candidate, Accumulation of demographic data after rejecting a candidate or presenting an offer)
- Multiple different front end views for different types of user
