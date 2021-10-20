# creatingANodeModuleFromScratch
Creating a node module from scratch by : Jaswant Chaudhary

#STEP:1 -> ### Create a parent folder inside which you want to create node_module, let's sy parent folder name is <CreateNodeModuleProject>
  
#STEP:2 -> ### Now navigate inside the folder <CreateNodeModuleProject>, by using command : < cd CreateNodeModuleProject >
  
#STEP:3 -> ### Now run the following command in the terminal : < npm init >
  
#STEP:4 -> ### Once you will run above command it will ask you the name of package file, give it a name : <package.json>
  
#STEP:5 -> ### Now it will ask you so many permission, just keep pressing enter button
  
#STEP:5 -> ### Now run the following command : <npm install -g json-server> 
  
#NOTE: If above command of STEP:5 Doesn't work, then run the following command <npm install json-server>

#STEP:6 -> ### Now create a file named : < db.json> , inside the parent directory <CreateNodeModuleProject>

#STEP:7 -> Now put this structire inside the < db.json > file :
                                                                {
                                                                
                                                                   "posts": [
                                                                    
                                                                              { "id": 1, "title": "json-server", "author": "typicode" }
                                                                  
                                                                    ],
                                                                  
                                                                    "comments": [
                                                                   
                                                                                { "id": 1, "body": "some comment", "postId": 1 }
                                                                  
                                                                     ],
                                                                  
                                                                      "profile": { "name": "typicode" }
                                                                
                                                                    }
  
#STEP:8 -> Now run the following command into your terminal : < json-server --watch db.json > 
  
#NOTE : If above command of STEP:8 Doesn't work then run the following command : < npx json-server --watch db.json >

#STEP:9 -> Now if you go to http://localhost:3000/posts/1, you'll get the following outPut : 

                    { "id": 1, "title": "json-server", "author": "typicode" }

