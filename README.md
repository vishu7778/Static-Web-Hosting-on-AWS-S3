Hosting a Carvilla Website on AWS S3 Service
--
Step 1: Create S3 Bucket:
1. Open the AWS Management Console
2. Navigate to S3 under the Services section
3. Click on “Create bucket”
4. Name the bucket `demo-static-website-15` (Bucket names must be
globally unique).

--

Step 2: Upload Website Files:
1. After creating the bucket, go inside it
2. Click on the Upload button.
3. Upload all your website's static files — like `index.html`, `styles.css`,
`script.js`, images, etc.(Carvilla,Free CSS Templates)

--

Step 3: Enable Bucket Versioning:
1. Go to the Properties tab of the bucket
2. Scroll to the Bucket Versioning section
3. Click Edit and enable versioning

--

Step 4: Enable Static Web Hosting:
1. In the Properties tab, scroll to Static website hosting
2. Click Edit, then:
- Select Enable.
- Set the Index document to `index.html`
- (Optional) Set an error document like `error.html`

--

Step 5: Unblock Public Access:
1. Go to the Permissions tab
2. Click on Block public access (bucket settings)
3. Click Edit, uncheck all options to disable blocking public access
4. Confirm the warning and save

--

Step 6: Change Object Ownership & Enable Ownership:
1. Still under Permissions, go to Object Ownership
2. Click Edit and select ACLs enabled (bucket owner preferred or object writer preferred).

--

Step 7: Make Uploaded File Public Using ACL:
1. Go to the Objects,Select all files and click Actions → Make public
2. Confirm the action,Each object will now have a public URL accessible via browser

--

Step 8: Access the Static Website:
After enabling hosting and permissions, your site can be accessed at:
http://demo-static-website-15.s3-website.ap-south-1.amazonaws.com

Here, Carvilla Website Hosted Successfully..
