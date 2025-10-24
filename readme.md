## Active Pieces / Sellsy
Simple automation d'exemple pour appliquer les CF d'une company sur une nouvelle facture.

![image info](./pic.png)

```javascript
export const code = async (inputs) => {
  return inputs.data.map(item => "embed[]=cf." + item.id).join("&");
};
```