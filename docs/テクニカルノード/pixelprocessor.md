---
sidebar_position: 1
---

# Pixelprocessor
###### (ピクセルプロセッサー)
export const Highlight = ({children, color}) => (
  <span
    style={{
      backgroundColor: color,
      borderRadius: '20px',
      color: '#fff',
      padding: '10px',
      cursor: 'pointer',
    }}
    onClick={() => {
      alert(`You clicked the color ${color} with label ${children}`)
    }}>
    {children}
  </span>
);

<Highlight color="#25c2a0">甘口</Highlight>

## 概要
ピクセル単位で計算を行い、結果を返します。

## 詳細
後で書く

:::tip ヒント

アドビ公式サイトに、基本的なノードの解説が載っています。  
公式サイトに載っているものは、そちらを参照するのもよいと思います。  
[アドビ公式サイトを見る](http://localhost:3000/my-react-page)

:::
