## API Routes for Comments Component

- Create : Adds comment to database
  - Type = POST
  - Url = `song/:id/comment`
  - Req.body = {comment-text, songTimeStamp, postDate, parentCommentId, userId}
  - Returns = None 
- Read: Gets all comments for specific page
  - Type = GET
  - Url = `song/:id/comments`
  - Returns = array of comments for the page 

- Update: Updates a comment (when user edits)
  - Type = PATCH 
  - Url = `song/:id/comment/:comment_id`
  - Req.body = {comment_text: newComment, userId}
  - Returns = None

- Delete: Remove comment/ all its replies
  - Type = DELETE
  - Req.body = {userId}
  - Url = `song/:id/comment/:comment_id`
  - Returns = None



