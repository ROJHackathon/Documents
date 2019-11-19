# API

## login
* login (token, password, time)
* login_status (user_name)

## register
* make_user (user_name, password, email, native, preference)

## feed
* request_feed (uid)
* search_material (keyword, uid)
* comment (uid, material_id, comment)
* like (uid, material_id)
* get_like (material_id)
* get_comment (material_id)

## translate
* translate_sentence (sentence)
* translate_sentence_smart (sentence, situation, age, tense)
* dictionary (word)

## chatroom
* get_chatroom_list (uid)
* create_chatroom (uid, isPrivate, name, members)
* say (uid, chatroom_id, text)
* update_chatroom (uid, chatroom_id)
* get_active_user (uid, chatroom_id, time)