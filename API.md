# API

## login
* login (token, password, time) -> code:int
* login_status (user_name) -> code:int

## register
* make_user (user_name, password, email, native, preference) -> code:int
* setEmail (uid, email) -> code:int
* setLanguage (uid, language) -> code:int
* setPreference (uid, preference) -> code:int

## feed
* request_feed (uid) -> materialList:Material[]
* search_histry (uid) -> historyList:String[]
* search_top_word () -> topwordList:String[]
* search_material (keyword, uid) -> materialList:Material[]
* comment (uid, material_id, comment) -> code:int
* like (uid, material_id) -> code:int
* get_like (material_id) -> likeNum:int
* get_comment (material_id) -> commentList:Comment[]


## translate
* translate_sentence (sentence) -> translation:String
* translate_sentence_smart (sentence, situation, age, tense) -> translation:String
* dictionary (word) -> record:Record

## chatroom
* get_chatroom_list (uid) -> chatroomList:Chatroom
* create_chatroom (uid, isPrivate, name, members) -> code:int
* say (uid, chatroom_id, text) -> code:int
* update_chatroom (uid, chatroom_id) -> commentList:Comment[]
* get_active_user (uid, chatroom_id, time) -> userList:User[]

## Code
* 0 -> fail
* 1 -> success