<table><tr><td> <em>Assignment: </em> IT202 Milestone 3 API Project</td></tr>
<tr><td> <em>Student: </em> Harsh Patel (hp548)</td></tr>
<tr><td> <em>Generated: </em> 8/8/2023 1:47:53 AM</td></tr>
<tr><td> <em>Grading Link: </em> <a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IT202-450-M23/it202-milestone-3-api-project/grade/hp548" target="_blank">Grading</a></td></tr></table>
<table><tr><td> <em>Instructions: </em> <ol><li>Checkout Milestone3 branch</li><li>Create a new markdown file called milestone3.md</li><li>git add/commit/push immediate</li><li>Fill in the below deliverables</li><li>At the end copy the markdown and paste it into milestone3.md</li><li>Add/commit/push the changes to Milestone3</li><li>PR Milestone3 to dev and verify</li><li>PR dev to prod and verify</li><li>Checkout dev locally and pull changes just to be up to date</li><li>Submit the direct link to this new milestone3.md file from your GitHub prod branch to Canvas</li></ol><p>Note: Ensure all images appear properly on github and everywhere else. Images are only accepted from dev or prod, not local host. All website links must be from prod (you can assume/infer this by getting your dev URL and changing dev to prod).</p></td></tr></table>
<table><tr><td> <em>Deliverable 1: </em> API Data Association </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="https://user-images.githubusercontent.com/54863474/211707773-e6aef7cb-d5b2-4053-bbb1-b09fc609041e.png"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Consider how your API data will be associated with a user</td></tr>
<tr><td> <em>Response:</em> <div>1. From the API, the quotes will be saved to another table name<br>"favourites" along with the user_id. So that the quotes don't get mixed up<br>with other users. By clicking on get a quotes it generates random quotes<br>and when the user click on the heart button It goes in to<br>the favourites table and user is redirected to the favorites pages.</div><div><br></div><div>2. When the<br>user edit a quotes meaning add a few lines into the quote. The<br>quote became associated with the user and he sees a new version of<br>the quote and not the previous ones. The main logic and reasoning behind<br>is that to make user not be able to fabricate the original quotes<br>of the person. When he clicks on the edit button and add a<br>few lines the whole quote became associated with himself</div><br></td></tr>
<tr><td> <em>Sub-Task 2: </em> Handling Data Changes</td></tr>
<tr><td> <em>Response:</em> <div>1)</div><div>When the data is being fetched by the API the user will see<br>all of it's entities in the favorites page. There we give the option<br>to the user to either update or delete the content. When the user<br>click on update button and tries to update the content. And suceeded to<br>finally add some lines in the existing quote. The quote author changes to<br>the user's name itself. To identify that this is users content.</div><div><br></div><div>2)</div><div>1- The script<br>initiates a fresh session or resumes a pre-existing one by utilizing the session_start()<br>function.</div><div>2- The code verifies whether the user_id variable has been assigned a value<br>in the session. If the user's credentials are not verified, they will be<br>automatically forwarded to the login page.</div><div>3- The script subsequently incorporates the common_functions.php file,<br>which is expected to contain the updateUser function.</div><div>4- The script verifies whether the<br>update field has been assigned a value in the POST data. If the<br>user's request does not meet the specified criteria, they will be automatically sent<br>to the index page.</div><div>5- In the event that the update field is enabled,<br>the script proceeds to extract the user_id, name, email, and password from the<br>POST data.</div><div>6- The program verifies whether any of the aforementioned fields are devoid<br>of content. In the event that the specified conditions are met, an error<br>message is established within the session, subsequently resulting in the user being redirected<br>to the index page.</div><div>7- When all the fields are completed, the script invokes<br>the updateUser method, passing the user_id, name, email, and password as arguments.</div><div>8- If<br>the updateUser function successfully executes, a message indicating success is stored in the<br>session. In the event that the return value is false, an error message<br>is established within the session.</div><div>9- Ultimately, the user is sent to the index<br>page.</div><div><br></div><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 2: </em> Handle the association of data to a user </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="https://user-images.githubusercontent.com/54863474/211707834-bf5a5b13-ec36-4597-9741-aa830c195be2.png"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Which option did you need to do to handle the association of data?</td></tr>
<tr><td> <em>Response:</em> <div>Within the code implementation, when the update field is specified in the POST<br>data, it triggers the process of modifying the user's information, encompassing attributes such<br>as name, email, and password, within the system. This suggests that the user<br>possesses agency over their own data, and the update mechanism enables them to<br>make modifications to the data linked to them. In contrast, Option 2 entails<br>the establishment of a webpage wherein an individual of higher authority, such as<br>a superior, have the ability to allocate associations to the user's data. In<br>this scenario, the user lacks power over their own data, resembling a system<br>based on roles.</div><div><br></div><div>So. I've used option 1.</div><br></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add screenshots of the updated/created pages related to associating data with the user (include code screenshots)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T18.37.44image.png.webp?alt=media&token=e3c1ade4-f05e-45f7-b7f6-0c323603a704"/></td></tr>
<tr><td> <em>Caption:</em> <p>Here it shows the role protected page.<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T18.39.00image.png.webp?alt=media&token=1488ec8f-d411-4f06-8dd7-1599d94753e5"/></td></tr>
<tr><td> <em>Caption:</em> <p>Here user can handle it&#39;s own data like as explained above<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Include any Heroku prod links to pages that would trigger entity to user association</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/user/account_page.php">https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/user/account_page.php</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Include any PRs related to this task</td></tr>
<tr><td>Not provided</td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 3: </em> Logged in user’s associated entities page </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="https://user-images.githubusercontent.com/54863474/211707834-bf5a5b13-ec36-4597-9741-aa830c195be2.png"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> What is the data that's associated with the user?</td></tr>
<tr><td> <em>Response:</em> <div>User ID: Each user in the system most likely has a unique identifier<br>like this. It is used to retrieve and modify user information and is<br>kept in the $_SESSION["user_id"] variable.&nbsp;</div><div>Name: The $user['name'] variable contains the user's name.</div><div>Email: The<br>$user['email'] variable contains the user's email address.</div><div>Password: The $user['password'] variable contains the user's<br>password.</div><div>Both the account_page.php file and the update_user.php file employ these bits of information<br>to show and update the user's information, respectively. Through the form on the<br>account page, the user can change their name, email address, and password.</div><div><br></div><div>An "entity"<br>is frequently used in the context of a software system to refer to<br>an important thing or idea, typically related to a person, location, thing, or<br>event. In this scenario, the "User" would be regarded as an entity, and<br>its associated information (User ID, Name, Email, and Password) would serve as its<br>characteristics.</div><br></td></tr>
<tr><td> <em>Sub-Task 2: </em> Show screenshots of the logged in user's entities associated with them  (include code screenshots)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.10.44image.png.webp?alt=media&token=e895bc8b-37dd-4df2-9bfb-b9db951851a8"/></td></tr>
<tr><td> <em>Caption:</em> <p>There 2 things things associated with the use, it&#39;s names and the quote<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.11.48image.png.webp?alt=media&token=2321d7fa-05c5-4942-95b4-8fee73b802fc"/></td></tr>
<tr><td> <em>Caption:</em> <p>This is the account details and user can edit them as they like<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.13.33image.png.webp?alt=media&token=b0c9af02-9e72-47ef-8c1a-cc191a98df33"/></td></tr>
<tr><td> <em>Caption:</em> <p>Admin page where it can see all the data of the users and<br>it sure can edit and remove any desired of them<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.14.37image.png.webp?alt=media&token=c78e118d-0041-4e0d-8f9a-6496ad661989"/></td></tr>
<tr><td> <em>Caption:</em> <p>These are the current admin page. if you click on edit it will<br>take you to respective page where you can edit<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add Heroku Prod links to the page(s) where the logged in user has their entities listed</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/user/account_page.php">https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/user/account_page.php</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Include any PRs related to this task</td></tr>
<tr><td>Not provided</td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 4: </em> All Users association page (Note: This will likely be an admin page and is not the same as the previous item) </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="https://user-images.githubusercontent.com/54863474/211707834-bf5a5b13-ec36-4597-9741-aa830c195be2.png"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Describe/Explain the purpose of this page from your project perspective</td></tr>
<tr><td> <em>Response:</em> <p>The &quot;admin.php&quot; page in your project appears to be responsible for retrieving all<br>users from the database. This page is likely used by administrators to manage<br>or view all users in the system.<br></p><br></td></tr>
<tr><td> <em>Sub-Task 2: </em> Show screenshots of the entity data associated with many users (include code screenshots)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.27.10image.png.webp?alt=media&token=1266cf4e-90c9-4aed-ba2f-966c7466a69d"/></td></tr>
<tr><td> <em>Caption:</em> <p>The page that has all the things in it<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.27.46image.png.webp?alt=media&token=dc45fffd-9e1a-4f70-b922-09842f4afe5c"/></td></tr>
<tr><td> <em>Caption:</em> <p>We can apply filters to the user data<br></p>
</td></tr>
<tr><td>Missing Image</td></tr>
<tr><td> <em>Caption:</em> <p>It has filter by options<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.29.21image.png.webp?alt=media&token=fcb228a7-edcf-428f-b545-04f4d2377ba8"/></td></tr>
<tr><td> <em>Caption:</em> <p>Also had sort by option<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.30.07image.png.webp?alt=media&token=4425af52-87bc-4b81-a6bc-a912f1bf6e94"/></td></tr>
<tr><td> <em>Caption:</em> <p>code snippet<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add Heroku Prod links to the page(s) where entities associated to many users can be seen</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/favourites/favourites_page.php">https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/favourites/favourites_page.php</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Include any PRs related to this task</td></tr>
<tr><td>Not provided</td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 5: </em> Create a page that shows data not associated with any user (Note: This will likely be an admin page and is not the same as the previous item) </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="https://user-images.githubusercontent.com/54863474/211707834-bf5a5b13-ec36-4597-9741-aa830c195be2.png"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Show screenshots of the page showing entities not associated with anyone (include code screenshots)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.40.50image.png.webp?alt=media&token=211e98a1-a0f0-4b48-a740-17c0f4149aea"/></td></tr>
<tr><td> <em>Caption:</em> <p>As my program is user driven, the users have more hold on the<br>data than an admin.  This is the screenshot that represent the main<br>things asked above<br></p>
</td></tr>
<tr><td><img width="768px" src="https://firebasestorage.googleapis.com/v0/b/learn-e1de9.appspot.com/o/assignments%2Fhp548%2F2023-08-07T20.41.18image.png.webp?alt=media&token=fe7981b0-cc9c-4799-9e3a-b6dc3028f809"/></td></tr>
<tr><td> <em>Caption:</em> <p>This is the code that is responsible for user un-association<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add Heroku Prod links to the page(s) where unassociated entities can be seen</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/admin/admin_page.php">https://hp548-project-prod-bfa623f3d3c6.herokuapp.com/admin/admin_page.php</a> </td></tr>
<tr><td> <em>Sub-Task 3: </em> Include any PRs related to this task</td></tr>
<tr><td>Not provided</td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 6: </em> Admin can associate any entity with any users (Note: This may be a form on an existing association page if you rather not have a separate page for this) </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="https://user-images.githubusercontent.com/54863474/211707795-a9c94a71-7871-4572-bfae-ad636f8f8474.png"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshots showing evidence of the checklist items (include code screenshots)</td></tr>
<tr><td><table><tr><td>Missing Image</td></tr>
<tr><td> <em>Caption:</em> (missing)</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Explain the code logic for this page</td></tr>
<tr><td> <em>Response:</em> <p>(missing)</p><br></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add Heroku Prod links to the page(s) related to this task</td></tr>
<tr><td>Not provided</td></tr>
<tr><td> <em>Sub-Task 4: </em> Include any PRs related to this task</td></tr>
<tr><td>Not provided</td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 7: </em> Reflection </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="https://user-images.githubusercontent.com/54863474/211707773-e6aef7cb-d5b2-4053-bbb1-b09fc609041e.png"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Document any issues/struggles</td></tr>
<tr><td> <em>Response:</em> <div>One of the main challenges I faced during the project was implementing the<br>association feature in the admin page. It was difficult to figure out how<br>to create a form that could handle partial matches and display the results<br>in a user-friendly way.</div><div>I overcame this issue by doing additional research on SQL<br>queries and form handling in PHP. I also sought advice from more experienced<br>developers in online communities, which helped me understand how to structure my code<br>and handle edge cases.</div><br></td></tr>
<tr><td> <em>Sub-Task 2: </em> Highlight any favorite topics</td></tr>
<tr><td> <em>Response:</em> <p>I particularly enjoyed working with SQL databases during this project. It was satisfying<br>to see how the data from the database could be used to create<br>dynamic, interactive features on the web pages. I also enjoyed learning more about<br>PHP and how it can be used to handle form submissions and interact<br>with a database.<br></p><br></td></tr>
<tr><td> <em>Sub-Task 3: </em> Overall how do you feel you did with the project and meeting requirements</td></tr>
<tr><td> <em>Response:</em> <p>Overall, I feel that I did well with the project. While there were<br>some challenges along the way, I was able to overcome them and learn<br>a lot in the process. I believe I met most of the project<br>requirements, although there are a few areas where I could improve in future<br>projects.<br></p><br></td></tr>
<tr><td> <em>Sub-Task 4: </em> Summarize your experience per the checklist items</td></tr>
<tr><td> <em>Response:</em> <p><img src="" alt="">When I started the class, I had some basic development experience<br>but had not worked extensively with PHP or SQL.<div class="col">Now, I feel much<br>more confident in my development skills. I have a better understanding of how<br>to structure a project, write efficient code, and debug issues.</div><div class="col">If I were<br>to do this project again, I would spend more time planning the structure<br>of the project before starting to code. I found that some issues could<br>have been avoided with better planning.</div><div class="col">Overall, this project was a valuable learning<br>experience. I improved my development skills, learned how to overcome challenges, and gained<br>a better understanding of how to create a dynamic, interactive web application.</div><br></p><br></td></tr>
</table></td></tr>
<table><tr><td><em>Grading Link: </em><a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IT202-450-M23/it202-milestone-3-api-project/grade/hp548" target="_blank">Grading</a></td></tr></table>