# React Chat Log

A chat log components with react.

## Usage

```tsx
import ReactChatLog, { Image, Link, Text } from 'react-chat-log'

function App() {

  const datas = [
    {
      msgType: 'text',
      content: 'hola'
    }, 
    {
      msgType: 'link',
      content: {
        title: 'Lorem jisldp',
        desc: 'Lorem jisldp dsd oor',
        img: 'https://picsum.photos/200/300',
        href: 'https://picsum.photos/200/300'
      }
    }, 
    {
      msgType: 'image',
      content: 'https://picsum.photos/200/300'
    }
  ]
  
  return (
    <ReactChatLog 
      datas={datas} 
      width={400}
      height={600}
    />
  )
}
```
