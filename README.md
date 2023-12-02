import random
from "PIL" import Image

letters = [
    "Mahal kita nang sobra-sobra!",
    "Ikaw ang nagbibigay ng kulay sa buhay ko.",
    "Kahit anong mangyari, nandito lang ako para sa 'yo.",
    "Ang ganda mo kapag ngumingiti ka.",
    "Salamat sa pagmamahal at suporta mo sa akin.",
    "Ikaw ang pinakamagandang nangyari sa buhay ko.",
    "Hindi ko kayang mawala ka sa aking buhay.",
    "Kahit saan man tayo mapunta, lagi kang nasa puso ko.",
    "Ikaw ang aking inspirasyon at lakas.",
    "Walang katulad ang pagmamahal ko para sa 'yo."
]

def show_random_letter_with_image():
    random_letter = random.choice(letters)
    print(random_letter)
    image_path = "Videoframe_20231203_015054_com.huawei.himovie.overseas.jpg"  # Palitan ng tamang path papunta sa larawan ng iyong girlfriend
    image = Image.open(image_path)
    image.show()

# Main program loop
while True:
    user_input = input("Pindutin ang Enter para makita ang sulat at larawan o i-type ang 'quit' para lumabas: ")
    if user_input.lower() == "quit":
        break
    else:
        show_random_letter_with_image()
