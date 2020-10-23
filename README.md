# React Chat Log

A chat log components with react.

## Usage

```tsx
import ReactChatLog from 'react-chat-log'

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
      initIndex={10} 
      width={400}
      height={600}
      onReachTop={() => console.log('it top')}
      onScroll={offsetTop => console.log(offsetTop)} 
      renderText={item => {}}
      renderLink={item => {}}
      renderImage={item => {}}
    />
  )
}
```
