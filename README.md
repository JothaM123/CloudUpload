# CloudUpload
This is the official CloudUpload website
 
 # Source Code
 ```python
 
        import os
        import pyimgur

        USER_ID = "YOUR_USER_ID"

        print("""
        █▀▀ █   █▀▀█ █  █ █▀▀▄ █  █ █▀▀█ █   █▀▀█ █▀▀█ █▀▀▄
        █   █   █  █ █  █ █  █ █  █ █  █ █   █  █ █▄▄█ █  █
        ▀▀▀ ▀▀▀ ▀▀▀▀ ▀▀▀▀ ▀▀▀  ▀▀▀▀ █▀▀▀ ▀▀▀ ▀▀▀▀ ▀  ▀ ▀▀▀
        """)
        size= os.get_terminal_size().columns
        print("─"*size)

        imgur = pyimgur.Imgur(USER_ID)


        while 1:
            FILE = input("📄 Enter Your File Path With Extension.")
            TITLE = input("🔤 Enter Title")
            image = imgur.upload_image(FILE, title=TITLE)
            print("🔗 Uploaded Link : " + image.link)
            input("⌨️ Please Hit Enter To Upload Another Image...")
 
 ```
