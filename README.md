# Text-to-Emoji
Text to Emoji

#### Python Code:

```

def text_to_emoji(text):
    emoji_mapping = {
        "love": "❤️",
        "pizza": "🍕",
        "beach": "🏖️",
        "ice cream": "🍦",
        "smile": "😊",
        "try": "😃",
        # Add more mappings as needed
    }
    
    emoji_coded_text = text
    for word, emoji in emoji_mapping.items():
        emoji_coded_text = emoji_coded_text.replace(word, emoji)
    
    return emoji_coded_text

def main():
    while True:
        text_input = input("Enter the text you want to convert into emoji code (or 'exit' to quit): ")
        if text_input.lower() == 'exit':
            break
        
        emoji_coded_text = text_to_emoji(text_input)
        print("Emoji code:", emoji_coded_text)

if __name__ == "__main__":
    main()


```
