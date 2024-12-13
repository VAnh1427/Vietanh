import time
import sys

def type_writer_effect(text, delay=0.05):
    for char in text:
        sys.stdout.write(char)
        sys.stdout.flush()
        time.sleep(delay)
    print()

def heart_art():
    art = """
      *****       *****
    **     **   **     **
   **       ** **       **
   **        ***        **
    **                 **
      **             **
        **         **
          **     **
            ** **
             ***
              *
    """
    print(art)

def secret_love_story():
    story = """
    Chào bạn,
    Nếu bạn đang đọc những dòng này, có lẽ bạn đã vô tình (hoặc cố ý) khám phá một bí mật giấu kín trong repo này...

    Mọi dòng code, mọi commit đều mang theo một thông điệp:

        "Mình đã thích bạn từ rất lâu rồi. ❤️"

    Dù đây chỉ là một đoạn mã nhỏ, nhưng mình hy vọng nó sẽ làm bạn mỉm cười.

    Nếu bạn cũng có chút gì đó dành cho mình, hãy để lại một ngôi sao ⭐ nhé.

    """
    type_writer_effect(story, delay=0.07)

if __name__ == "__main__":
    type_writer_effect("Đang tải bí mật...", delay=0.1)
    time.sleep(1)
    type_writer_effect("3...", delay=0.5)
    time.sleep(0.5)
    type_writer_effect("2...", delay=0.5)
    time.sleep(0.5)
    type_writer_effect("1...", delay=0.5)
    time.sleep(0.5)
    heart_art()
    secret_love_story()
