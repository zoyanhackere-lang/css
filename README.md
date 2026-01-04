# css
all-tools-website
<!DOCTYPE html><html><head><meta charset='UTF-8'><title>30 All Tools – Zoyan Hackere</title><style>body{font-family:Arial;background:#0f172a;color:white;margin:0}header{background:#2563eb;padding:15px;text-align:center;font-size:24px}.tools{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:15px;padding:20px}.tool{background:#1e293b;padding:15px;border-radius:10px}h3{margin:0 0 8px}input,textarea,select,button{width:100%;padding:7px;margin:4px 0;border-radius:6px;border:none}button{background:#22c55e;cursor:pointer}.res{color:#a7f3d0;font-size:14px}</style></head><body><header>🛠️ 30 All-in-One Tools (Fully Usable)</header><div class='tools'>
<div class='tool'><h3>1 Password Generator</h3><button onclick="pg()">Generate</button><div class='res' id='pg'></div></div>
<div class='tool'><h3>2 Text Counter</h3><textarea id='tc'></textarea><button onclick="tcf()">Count</button><div class='res' id='tcr'></div></div>
<div class='tool'><h3>3 Word Counter</h3><textarea id='wc'></textarea><button onclick="wcf()">Count</button><div class='res' id='wcr'></div></div>
<div class='tool'><h3>4 Age Calculator</h3><input type='date' id='age'><button onclick="agef()">Calc</button><div class='res' id='ager'></div></div>
<div class='tool'><h3>5 BMI Calculator</h3><input id='bw' placeholder='kg'><input id='bh' placeholder='cm'><button onclick="bmif()">Calc</button><div class='res' id='bmir'></div></div>
<div class='tool'><h3>6 Random Number</h3><input id='rmin'><input id='rmax'><button onclick="randf()">Gen</button><div class='res' id='randr'></div></div>
<div class='tool'><h3>7 Base64 Encode</h3><textarea id='b64e'></textarea><button onclick="b64ef()">Encode</button><div class='res' id='b64er'></div></div>
<div class='tool'><h3>8 Base64 Decode</h3><textarea id='b64d'></textarea><button onclick="b64df()">Decode</button><div class='res' id='b64dr'></div></div>
<div class='tool'><h3>9 Stopwatch</h3><button onclick="sws()">Start</button><button onclick="swp()">Stop</button><div class='res' id='sw'>0</div></div>
<div class='tool'><h3>10 Timer (10s)</h3><button onclick="timer()">Start</button><div class='res' id='tr'></div></div>
<div class='tool'><h3>11 Notes</h3><textarea id='note'></textarea><button onclick="saveN()">Save</button><div class='res' id='noter'></div></div>
<div class='tool'><h3>12 Color Picker</h3><input type='color' id='cp'><div class='res' id='cpr'></div></div>
<div class='tool'><h3>13 Unit Converter (cm→m)</h3><input id='uc'><button onclick="ucf()">Convert</button><div class='res' id='ucr'></div></div>
<div class='tool'><h3>14 Currency (PKR→USD)</h3><input id='cur'><button onclick="curf()">Convert</button><div class='res' id='curr'></div></div>
<div class='tool'><h3>15 Loan Calculator</h3><input id='loan'><button onclick="loanf()">Calc</button><div class='res' id='loanr'></div></div>
<div class='tool'><h3>16 Text Encrypt</h3><textarea id='enc'></textarea><button onclick="encf()">Encrypt</button><div class='res' id='encr'></div></div>
<div class='tool'><h3>17 Text Decrypt</h3><textarea id='dec'></textarea><button onclick="decf()">Decrypt</button><div class='res' id='decr'></div></div>
<div class='tool'><h3>18 Fake Name</h3><button onclick="namef()">Gen</button><div class='res' id='namer'></div></div>
<div class='tool'><h3>19 Text to Upper</h3><textarea id='up'></textarea><button onclick="upf()">Convert</button><div class='res' id='upr'></div></div>
<div class='tool'><h3>20 Text to Lower</h3><textarea id='low'></textarea><button onclick="lowf()">Convert</button><div class='res' id='lowr'></div></div>
<div class='tool'><h3>21 Character Remover</h3><textarea id='rem'></textarea><input id='char'><button onclick="remf()">Remove</button><div class='res' id='remr'></div></div>
<div class='tool'><h3>22 Text Reverse</h3><textarea id='rev'></textarea><button onclick="revf()">Reverse</button><div class='res' id='revr'></div></div>
<div class='tool'><h3>23 Percentage Calc</h3><input id='per'><button onclick="perf()">Calc</button><div class='res' id='perr'></div></div>
<div class='tool'><h3>24 Number Square</h3><input id='sq'><button onclick="sqf()">Calc</button><div class='res' id='sqr'></div></div>
<div class='tool'><h3>25 Number Cube</h3><input id='cb'><button onclick="cbf()">Calc</button><div class='res' id='cbr'></div></div>
<div class='tool'><h3>26 Even/Odd</h3><input id='eo'><button onclick="eof()">Check</button><div class='res' id='eor'></div></div>
<div class='tool'><h3>27 URL Encoder</h3><input id='url'><button onclick="urlf()">Encode</button><div class='res' id='urlr'></div></div>
<div class='tool'><h3>28 URL Decoder</h3><input id='urld'><button onclick="urldf()">Decode</button><div class='res' id='urldr'></div></div>
<div class='tool'><h3>29 Random Color</h3><button onclick="rcf()">Gen</button><div class='res' id='rcr'></div></div>
<div class='tool'><h3>30 Calculator</h3><input id='cal'><button onclick="calf()">Eval</button><div class='res' id='calr'></div></div>
</div><script>
function pg(){let c='abcABC123!@#';let p='';for(i=0;i<8;i++)p+=c[Math.random()*c.length|0];pg.innerText=p}
function tcf(){tcr.innerText=tc.value.length}
function wcf(){wcr.innerText=wc.value.split(/\s+/).filter(Boolean).length}
function agef(){ager.innerText=new Date().getFullYear()-new Date(age.value).getFullYear()}
function bmif(){bmir.innerText=(bw.value/((bh.value/100)**2)).toFixed(2)}
function randf(){randr.innerText=Math.floor(Math.random()*(+rmax.value-+rmin.value+1))+ +rmin.value}
function b64ef(){b64er.innerText=btoa(b64e.value)}function b64df(){b64dr.innerText=atob(b64d.value)}
let s=0,si;function sws(){si=setInterval(()=>sw.innerText=++s,1000)}function swp(){clearInterval(si)}
function timer(){let t=10;tr.innerText=t;let i=setInterval(()=>{t--;tr.innerText=t;if(t==0)clearInterval(i)},1000)}
function saveN(){localStorage.n=note.value;noter.innerText='Saved'}cp.oninput=()=>cpr.innerText=cp.value
function ucf(){ucr.innerText=uc.value/100}
function curf(){curr.innerText=(cur.value/280).toFixed(2)}
function loanf(){loanr.innerText=loan.value*1.1}
function encf(){encr.innerText=btoa(enc.value)}function decf(){decr.innerText=atob(dec.value)}
function namef(){let n=['Ali','Ahmed','Sara','Ayesha'];namer.innerText=n[Math.random()*n.length|0]}
function upf(){upr.innerText=up.value.toUpperCase()}function lowf(){lowr.innerText=low.value.toLowerCase()}
function remf(){remr.innerText=rem.value.split(char.value).join('')}
function revf(){revr.innerText=rev.value.split('').reverse().join('')}
function perf(){perr.innerText=per.value+'%'}function sqf(){sqr.innerText=sq.value*sq.value}
function cbf(){cbr.innerText=cb.value**3}function eof(){eor.innerText=eo.value%2?'Odd':'Even'}
function urlf(){urlr.innerText=encodeURIComponent(url.value)}function urldf(){urldr.innerText=decodeURIComponent(urld.value)}
function rcf(){let c='#'+Math.random().toString(16).slice(2,8);rcr.innerText=c}
function calf(){calr.innerText=eval(cal.value)}
</script></body></html>
