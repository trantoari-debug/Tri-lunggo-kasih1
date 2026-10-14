const http = require('http');
let seq = 0;
function genToken(){
  const t = Date.now()+seq++;
  const r = Math.floor(Math.random()*999999).toString().padStart(6,'0');
  return `B1-${t}-${r} | TRI LUNGGO KASIH | LIVE MERDEKA`;
}
http.createServer((req,res)=>{
  res.writeHead(200,{'Content-Type':'application/json'});
  res.end(JSON.stringify({server:"Tri Lunggo Merdeka Aktif", token:genToken()}, null, 2));
}).listen(process.env.PORT||3000);
