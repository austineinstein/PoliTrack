
Wikipedia For Nigerian Political events:

Ability to search political office holders based on name or position 

Ability to post stories given a user account

Upvote/Downvote stories

Creating a story requires a reference 

Homepage (Trending Topics for January/February..)

User log in 

A Value System for users

React + Firebase..


2/3 hours... per week!

Story
    id: string
    title: string
    date uploaded: dateTime
    link(s): list(string)
    personalitie(s): object(personalityId)
    comments: object
    countdown:int
    verifiedBy: object(userId)
    uploadedBy: userId
    
Comment
    id: string
    userId: string
    commentBody:string
    date: dateTime
    reply(ies): object{replyId, userId, replyText}

User
    userId: string
    email: email
    password: password
    dateJoined: dateTime
    valuePoints: int(number fo verified ids on story)

Admin
   adminId: string
   password: password

User--> Personality
    personalityId: string
    email:email
    name: string
    position: string
    dateJoined: dateTime
    dateInOffice: dateTime
    dateOutOfOffice: dateTime
    story: object(Story)
