










define y = Character('ยูกะ', color="#E259E2", what_color="#E259E2")
define k = DynamicCharacter('player_name', color="#54F23D", what_color="#54F23D")
define p = Character('???', color="#EA2A2A", what_color="#EA2A2A")
define t = Character('    ', color="#C6F46C", what_color="#C6F46C")
define n = Character('โนโนะ', color="#F48D1C", what_color="#F48D1C")


# The game starts here.
label start:

    image background 1 = "Bg_3244.png"
    scene background 1

    $ player_name = renpy.input("(โปรดใส่ชื่อของคุณ และกดปุ่ม Enter)")
    $ player_name = player_name.strip()
    
    if player_name == "":
        $ player_name= "102" #ถ้าผู้เล่นไม่ยอมพิมพ์ชื่อ โปรแกรมจะตั้งชื่อว่า 102 ให้แทน
    
    t "ชื่อของคุณคือ  [player_name]!!"
    
    image background 1 = "Bg_3244.png"
    scene background 1

    k "เตรียมตัวใว้นะครับ ตอนนั้นเดี๋ยวเราจะหนีไปด้วยกัน"
    
    image Nakano Yuka not speak = "Nakano Yuka pose 0f3.png"
    show Nakano Yuka not speak with dissolve
    
    y "ถ้างั้นชั้นจะไปหาของที่พอใช้ป้องกันตัวได้นะคะ"
    
    image black = "Bg_3001.png"
    scene black with dissolve
    
    y "ตรงนี้ดูเหมือนจะมีอะไรอยู่ด้วยล่ะค่ะ โปรดิวเซอร์"
    
    t "คุณได้รับกรรไกร 1 EA"
    
    image background 1 = "Bg_3244.png"
    scene background 1 with dissolve
    
    image Nakano Yuka not speak = "Nakano Yuka pose 0f3.png"
    show Nakano Yuka not speak
    
    t "ทันใดนั้น ยูกะก็เห็นเงาบางอย่างอยู่ใต้โต้ะ ยูกะตกใจมากจึงรีบวิ่งมาหาคุณ"
    
    y "โปรดิวเซอร์คะ... คือว่า... มีอะไรไม่รู้อยู่ใต้โต้ะน่ะค่ะ"
    
    k "งั้นเดี๋ยวผมไปดูให้นะครับ"
    
    hide Nakano Yuka not speak with dissolve
    
    image black = "Bg_3001.png"
    scene black with dissolve
    
    t "คุณค่อยๆเดินไปที่โต๊ะ โดยยูกะคอยเดินตามหลังอย่างช้าๆ"
    
    p "ไม่ไหวเเล้ว..."
    
    p "โมริคุโบะ... รู้งี้นอนอยู่ที่บ้านดีกว่า"
    
    n "ไม่อยากอยู่ที่นี่... เอ่อ... ช่วยพาโมริคุโบะ... ออกไปจากที่นี่ได้มั๊ย..."
    
    image background 1 = "Bg_3244.png"
    scene background 1 with dissolve
    
    image Nakano Yuka speak = "Nakano Yuka pose 0f4.png"
    show Nakano Yuka speak 
    
    image Morikubo Nono = "Morikubo Nono pose 0f7.png"
    show Morikubo Nono at right with dissolve
    
    y "คุณโมริคุโบะนี่นา ว่าเเต่คุณมาอยู่ที่นี่ได้ยังไง"
    
    n "มีคน... ไล่ตามมาตลอดเลย... กลัวเเล้ว..."
    
    y "คุณคงเจอเเบบเดียวกับเราสินะ มันเหมือนกับในหนังที่โควเมะจังดูบ่อยๆเลย"
    
    y "ที่เกี่ยวกับเชื้อไวรัสอะไรนี่เเหล่ะ"
    
    k "ไม่ต้องกลัวนะทั้งสองคนผมจะพยายามคิดหาทางรอดเอง"
    
    k "ว่าเเต่ คุณยูกะครับ พอจะจำได้มั๊ยครับว่าตอนนั้นพวกมันตามมากันกี่คน"
    
    y "น่าจะ 3 คนนะคะ ตอนนั้นก็ไม่ได้สังเกตน่ะค่ะ"
    
    k "ผมว่าตอนนี้น่าจะไม่มีพวกมันอยู่เเถวนี้เเล้วล่ะ"
    
    k "ถ้าค่อยๆย่องไปพวกมันน่าจะไม่รู้ตัวนะ"
    
    n "โมริคุโบะต้องไม่ไหวเเน่ๆ..."
    
    y "คุณโมริคุโบะ... ไม่ต้องห่วง เราไปด้วยกันต้องไม่เป็นไรเเน่ๆ"
    
    k "ใช่ครับ อีกอย่างการดูเเลไอดอลเป็นหน้าที่ของโปรดิวเซอร์อย่างผมครับ"
    
    y "ว่าเเต่ จะไปที่ไหนดีล่ะคะ?"
    
    menu:
     "ห้องรับประทานอาหาร":
      jump home
      
     "บนดาดฟ้า":
      jump book
         
     "ประตูทางออก":
      jump work
           
    label home: 
        y "ตาย"
        jump next

    label book:
        y "ตาย"
        jump next

    label work:
        y "ตาย"
        jump next
                     
    label next:
                     
    image background 1 = "Bg_3244.png"
    scene background 1 with dissolve
    
    t "เช้าวันต่อมา...."
    

    
    
    
    
    
    
    
    
    
    
    
    return
