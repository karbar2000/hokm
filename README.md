<!doctype html>
<html lang="fa" dir="rtl"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>ENGLISH_PAYAM_GHADIR</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;600;800&display=swap">
<style>
:root{--bg:#eef3f8;--cd:#fff;--tx:#12202f;--mu:#5b6b7c;--ac:#0d8f8d;--ac2:#f2a900;--ok:#16a34a;--bad:#dc2626;--bd:#d5dee8;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media(prefers-color-scheme:dark){:root:not([data-theme=light]){--bg:#0e1724;--cd:#17243a;--tx:#e8eef6;--mu:#93a4b8;--ac:#2cc4c0;--bd:#26364f;color-scheme:dark}}
:root[data-theme=dark]{--bg:#0e1724;--cd:#17243a;--tx:#e8eef6;--mu:#93a4b8;--ac:#2cc4c0;--bd:#26364f;color-scheme:dark}
*{box-sizing:border-box}html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--tx);font:16px/1.7 Vazirmatn,Tahoma,system-ui,sans-serif;padding-bottom:84px}
main{max-width:920px;margin:auto;padding:16px}
.en{direction:ltr;unicode-bidi:isolate;text-align:left}
.top{display:flex;justify-content:space-between;align-items:center;gap:8px;flex-wrap:wrap;padding:12px 16px;max-width:920px;margin:auto}
.chip{background:var(--cd);border:1px solid var(--bd);border-radius:99px;padding:2px 12px;font-weight:600;font-size:14px}
.card{background:var(--cd);border:1px solid var(--bd);border-radius:14px;padding:16px;margin:10px 0}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:12px}
.tile{background:var(--cd);border:1px solid var(--bd);border-radius:14px;padding:16px 10px;text-align:center;cursor:pointer;font:inherit;color:inherit;transition:transform .15s,border-color .15s}
.tile:hover{transform:translateY(-3px);border-color:var(--ac)}.tile b{display:block;font-size:34px;line-height:1.3}
.btn,.btn2,.opt,.sp{font:inherit;cursor:pointer;border-radius:10px;border:1px solid var(--ac)}
.btn{background:var(--ac);color:#04201f;padding:8px 18px;font-weight:700}.btn2{background:none;color:var(--tx);padding:8px 16px;border-color:var(--bd)}
.sp{background:none;color:var(--tx);border-color:var(--bd);padding:2px 9px}.sp:hover{border-color:var(--ac)}
.in,select{font:inherit;background:var(--bg);color:var(--tx);border:1px solid var(--bd);border-radius:10px;padding:9px 12px;width:100%;margin:6px 0}
select{width:auto;min-width:150px}.row{display:flex;gap:10px;flex-wrap:wrap;align-items:center;margin-top:10px}
.opts{display:grid;gap:8px;margin-top:10px}.opt{background:var(--bg);color:var(--tx);padding:10px 14px;border-color:var(--bd);text-align:start}
.opt.ok{background:var(--ok);color:#fff;border-color:var(--ok)}.opt.no{background:var(--bad);color:#fff;border-color:var(--bad)}
.bar{height:8px;background:var(--bd);border-radius:9px;overflow:hidden}.bar i{display:block;height:100%;background:linear-gradient(90deg,var(--ac),var(--ac2));transition:width .4s}
.mu,.mut{color:var(--mu)}.big{font-size:56px;text-align:center}.q{font-size:20px;font-weight:600}
.ex{display:flex;gap:10px;align-items:center;background:var(--cd);border:1px solid var(--bd);border-radius:12px;padding:8px 12px}.em{font-size:34px}
.fm{font-weight:600;color:var(--ac)}.bad{color:var(--bad)}.good{color:var(--ok)}
table{width:100%;border-collapse:collapse}td,th{padding:6px 8px;border-bottom:1px solid var(--bd);text-align:start}
nav{position:fixed;inset:auto 0 0 0;background:var(--cd);border-top:1px solid var(--bd);display:flex;justify-content:center;gap:2px;padding:6px 6px calc(6px + env(safe-area-inset-bottom,0px))}
nav button{flex:1;max-width:110px;background:none;border:0;color:var(--mu);font:12px Vazirmatn,sans-serif;cursor:pointer;border-radius:10px;padding:4px}nav b{display:block;font-size:20px}
nav .on{color:var(--ac);background:var(--bg)}
.hi{font-size:28px;font-weight:800;animation:in .7s ease both}@keyframes in{from{opacity:0;transform:translateY(14px)}}
.badge{background:var(--ok);color:#fff;border-radius:8px;padding:0 8px;font-size:13px}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
</style></head><body>
<div class="top" id="top"></div><main id="app"></main><nav id="nav"></nav>
<script>
const $=s=>document.querySelector(s),esc=s=>String(s).replace(/&/g,'&amp;').replace(/"/g,'&quot;').replace(/</g,'&lt;');
const sh=a=>[...a].sort(()=>Math.random()-.5),sample=(a,n)=>sh(a).slice(0,n),uniq=a=>[...new Set(a)];
const cap=s=>s[0].toUpperCase()+s.slice(1),art=w=>/^[aeio]/i.test(w)?'an':'a';
const LS={get(k,d){try{const v=localStorage.getItem('epq_'+k);return v?JSON.parse(v):d}catch(e){return d}},set(k,v){try{localStorage.setItem('epq_'+k,JSON.stringify(v))}catch(e){}}};
let D=Object.assign({name:'',xp:0,done:[],ex:[],di:[],mis:[],st:{},theme:'auto',rate:1,dc:''},LS.get('d',{}));
const save=()=>LS.set('d',D),lv=()=>Math.floor(Math.sqrt(D.xp/100))+1;
function say(t){try{speechSynthesis.cancel();const u=new SpeechSynthesisUtterance(t);u.lang='en-US';u.rate=+D.rate;speechSynthesis.speak(u)}catch(e){}}
const sp=t=>`<button class="sp" data-t="${esc(t)}" aria-label="Play audio">🔊</button>`;
/* ---------- DATA ---------- */
const TP={to_be:'Verb To Be',simple_present:'Simple Present',present_continuous:'Present Continuous',simple_past:'Simple Past',future:'Future (Will / Going to)',countries:'Countries',nationalities:'Nationalities',irregular:'Irregular Verbs',vocabulary:'Vocabulary'};
const GT=['to_be','simple_present','present_continuous','simple_past','future'];
const SUBJ=['I','You','He','She','We','They'],is3=s=>s=='He'||s=='She',low=s=>s=='I'?s:s.toLowerCase();
const be=(s,p)=>p?(s=='I'||is3(s)?'was':'were'):(s=='I'?'am':is3(s)?'is':'are');
const V=`play|plays|playing|played|football|⚽
work|works|working|worked|hard|💼
study|studies|studying|studied|English|📚
watch|watches|watching|watched|TV|📺
eat|eats|eating|ate|an apple|🍎
run|runs|running|ran|in the park|🏃
read|reads|reading|read|a book|📖
write|writes|writing|wrote|a letter|✉️
drink|drinks|drinking|drank|water|🥤
sleep|sleeps|sleeping|slept|early|😴
buy|buys|buying|bought|a new book|🛍️
go|goes|going|went|to school|🏫
see|sees|seeing|saw|a film|🎬
make|makes|making|made|a cake|🎂
take|takes|taking|took|a photo|📷`.split('\n').map(l=>{const a=l.split('|');return{v:a[0],s:a[1],g:a[2],p:a[3],o:a[4],e:a[5]}});
const IRR=`buy|bought|bought|خریدن
hear|heard|heard|شنیدن
make|made|made|ساختن
keep|kept|kept|نگه داشتن
have|had|had|داشتن
catch|caught|caught|گرفتن (گیر انداختن)
get|got|gotten/got|گرفتن / شدن
find|found|found|پیدا کردن
go|went|gone|رفتن
see|saw|seen|دیدن
eat|ate|eaten|خوردن
drink|drank|drunk|نوشیدن
write|wrote|written|نوشتن
read|read|read|خواندن
take|took|taken|گرفتن / بردن
give|gave|given|دادن
come|came|come|آمدن
run|ran|run|دویدن
sit|sat|sat|نشستن
speak|spoke|spoken|صحبت کردن
know|knew|known|دانستن
think|thought|thought|فکر کردن
say|said|said|گفتن
tell|told|told|گفتن (برای کسی)
teach|taught|taught|آموزش دادن
sleep|slept|slept|خوابیدن
leave|left|left|ترک کردن
begin|began|begun|شروع کردن
bring|brought|brought|آوردن
forget|forgot|forgotten|فراموش کردن
swim|swam|swum|شنا کردن
fly|flew|flown|پرواز کردن
sing|sang|sung|آواز خواندن
drive|drove|driven|رانندگی کردن
win|won|won|برنده شدن
lose|lost|lost|گم کردن / باختن
meet|met|met|ملاقات کردن
pay|paid|paid|پرداختن
send|sent|sent|فرستادن
build|built|built|ساختن (بنا کردن)`.split('\n').map(l=>l.split('|'));
/* name|flag|nationality|languages|capital|area(thousand km2)|population(million, ~2023) */
const C=`Spain|🇪🇸|Spanish|Spanish|Madrid|506|48
France|🇫🇷|French|French|Paris|551|68
Germany|🇩🇪|German|German|Berlin|357|84
Italy|🇮🇹|Italian|Italian|Rome|301|59
United Kingdom|🇬🇧|British|English|London|243|68
United States|🇺🇸|American|English|Washington, D.C.|9834|335
Canada|🇨🇦|Canadian|English, French|Ottawa|9985|40
Mexico|🇲🇽|Mexican|Spanish|Mexico City|1964|128
Brazil|🇧🇷|Brazilian|Portuguese|Brasília|8516|216
Argentina|🇦🇷|Argentine|Spanish|Buenos Aires|2780|46
Colombia|🇨🇴|Colombian|Spanish|Bogotá|1142|52
China|🇨🇳|Chinese|Mandarin Chinese|Beijing|9597|1410
Japan|🇯🇵|Japanese|Japanese|Tokyo|378|124
South Korea|🇰🇷|Korean|Korean|Seoul|100|52
India|🇮🇳|Indian|Hindi, English|New Delhi|3287|1430
Pakistan|🇵🇰|Pakistani|Urdu, English|Islamabad|881|240
Afghanistan|🇦🇫|Afghan|Dari, Pashto|Kabul|652|41
Iran|🇮🇷|Iranian|Persian (Farsi)|Tehran|1648|89
Iraq|🇮🇶|Iraqi|Arabic, Kurdish|Baghdad|438|45
Turkey|🇹🇷|Turkish|Turkish|Ankara|784|85
Azerbaijan|🇦🇿|Azerbaijani|Azerbaijani|Baku|86.6|10
Russia|🇷🇺|Russian|Russian|Moscow|17098|144
Ukraine|🇺🇦|Ukrainian|Ukrainian|Kyiv|603.5|38
Poland|🇵🇱|Polish|Polish|Warsaw|313|37
Greece|🇬🇷|Greek|Greek|Athens|132|10.4
Portugal|🇵🇹|Portuguese|Portuguese|Lisbon|92|10.4
Netherlands|🇳🇱|Dutch|Dutch|Amsterdam|41.5|17.9
Sweden|🇸🇪|Swedish|Swedish|Stockholm|450|10.5
Switzerland|🇨🇭|Swiss|German, French, Italian, Romansh|Bern|41.3|8.9
Ireland|🇮🇪|Irish|English, Irish|Dublin|70.3|5.3
Egypt|🇪🇬|Egyptian|Arabic|Cairo|1002|112
Saudi Arabia|🇸🇦|Saudi|Arabic|Riyadh|2150|36
South Africa|🇿🇦|South African|11 official languages (e.g. Zulu, Xhosa, Afrikaans, English)|Pretoria (executive capital)|1221|60
Nigeria|🇳🇬|Nigerian|English|Abuja|924|224
Kenya|🇰🇪|Kenyan|Swahili, English|Nairobi|580|55
Indonesia|🇮🇩|Indonesian|Indonesian|Jakarta|1905|277
Thailand|🇹🇭|Thai|Thai|Bangkok|513|66
Vietnam|🇻🇳|Vietnamese|Vietnamese|Hanoi|331|99
Australia|🇦🇺|Australian|English|Canberra|7692|26
New Zealand|🇳🇿|New Zealander|English, Māori, NZ Sign Language|Wellington|268|5.2`.split('\n').map(l=>{const a=l.split('|');return{n:a[0],f:a[1],nat:a[2],l:a[3],cap:a[4],a:+a[5],p:+a[6]}});
const N=c=>(['United States','United Kingdom','Netherlands'].includes(c.n)?'the ':'')+c.n,L0=c=>c.l.split(',')[0].replace(/ \(.*/,'');
const W={Family:`mother|👩|مادر
father|👨|پدر
brother|👦|برادر
sister|👧|خواهر
grandmother|👵|مادربزرگ
grandfather|👴|پدربزرگ
baby|👶|نوزاد`,Food:`apple|🍎|سیب
banana|🍌|موز
egg|🥚|تخم‌مرغ
pizza|🍕|پیتزا
cake|🎂|کیک
sandwich|🥪|ساندویچ
carrot|🥕|هویج
orange|🍊|پرتقال`,Animals:`cat|🐱|گربه
dog|🐶|سگ
horse|🐴|اسب
bird|🐦|پرنده
fish|🐟|ماهی
cow|🐄|گاو
rabbit|🐰|خرگوش
lion|🦁|شیر`,Jobs:`doctor|👨‍⚕️|پزشک
teacher|🧑‍🏫|معلم
pilot|🧑‍✈️|خلبان
farmer|🧑‍🌾|کشاورز
cook|🧑‍🍳|آشپز
firefighter|🧑‍🚒|آتش‌نشان
singer|🧑‍🎤|خواننده`,Transport:`car|🚗|ماشین
bus|🚌|اتوبوس
train|🚆|قطار
plane|✈️|هواپیما
bicycle|🚲|دوچرخه
ship|🚢|کشتی`};
const WL=[];Object.keys(W).forEach(k=>W[k]=W[k].split('\n').map(l=>{const a=l.split('|');const o={w:a[0],e:a[1],fa:a[2],t:k};WL.push(o);return o}));
/* ---------- SENTENCES / QUESTION BANK (topic strict) ---------- */
function sent(t,v,S,k){const o=v.o,l=low(S),h=is3(S);
 if(t=='simple_present')return k=='n'?`${S} ${h?'does':'do'} not ${v.v} ${o} every day.`:k=='q'?`${h?'Does':'Do'} ${l} ${v.v} ${o} every day?`:`${S} ${h?v.s:v.v} ${o} every day.`;
 if(t=='present_continuous')return k=='n'?`${S} ${be(S)} not ${v.g} ${o} now.`:k=='q'?`${cap(be(S))} ${l} ${v.g} ${o} now?`:`${S} ${be(S)} ${v.g} ${o} now.`;
 if(t=='simple_past')return k=='n'?`${S} did not ${v.v} ${o} yesterday.`:k=='q'?`Did ${l} ${v.v} ${o} yesterday?`:`${S} ${v.p} ${o} yesterday.`;
 return k=='n'?`${S} will not ${v.v} ${o} tomorrow.`:k=='q'?`Will ${l} ${v.v} ${o} tomorrow?`:`${S} will ${v.v} ${o} tomorrow.`}
const mk=(t,q,r,d)=>{d=uniq(d).filter(x=>x!=r).slice(0,3);return{type:'mc',t,q,r,o:sh([r,...d]),id:'m|'+t+q}};
function Q(t){const o=[];
 if(t=='to_be')SUBJ.forEach(S=>[0,1].forEach(p=>{const r=be(S,p),tm=p?'yesterday':'now',all=['am','is','are','was','were'];
  o.push(mk(t,`${S} ____ at home ${tm}.`,r,all));o.push(mk(t,`${S} ____ not at school ${tm}.`,r,all));o.push(mk(t,`____ ${low(S)} at the park ${tm}?`,cap(r),all.map(cap)))}));
 else if(GT.includes(t))V.forEach(v=>SUBJ.forEach(S=>{const h=is3(S),b=be(S),wb=S=='He'||S=='She'?'are':'is',Sq=`${S} ____ (${v.v}) ${v.o}`;
  if(t=='simple_present')o.push(mk(t,`${Sq} every day.`,h?v.s:v.v,[v.v,v.s,v.g,v.p,'to '+v.v]));
  if(t=='present_continuous')o.push(mk(t,`${Sq} now.`,`${b} ${v.g}`,[`${b} ${v.v}`,v.g,`${wb} ${v.g}`,`${b} ${v.p}`]));
  if(t=='simple_past'){o.push(mk(t,`${Sq} yesterday.`,v.p,[v.v,v.g,v.v+'ed',v.s]));o.push(mk(t,`Did ${low(S)} ____ ${v.o} yesterday? (${v.v})`,v.v,[v.p,v.g,v.s,v.v+'ed']))}
  if(t=='future'){o.push(mk(t,`${Sq} tomorrow.`,`will ${v.v}`,[`will ${v.p}`,`will ${v.g}`,`will to ${v.v}`,`${v.v} will`]));o.push(mk(t,`${S} ____ ${v.o} tonight. (be going to ${v.v})`,`${b} going to ${v.v}`,[`${b} going ${v.v}`,`${wb} going to ${v.v}`,`will going to ${v.v}`,`${b} going to ${v.g}`]))}}));
 else if(t=='countries')C.forEach(c=>{o.push(mk(t,`${c.f} The capital of ${N(c)} is ____.`,c.cap,sample(C,6).map(x=>x.cap)));
  o.push(mk(t,`${c.f} One main language of ${N(c)} is ____.`,L0(c),C.filter(x=>!c.l.includes(L0(x))).map(L0)))});
 else if(t=='nationalities')C.forEach(c=>{o.push(mk(t,`${c.f} He is from ${N(c)}. He is ____.`,c.nat,sample(C,6).map(x=>x.nat)));o.push(mk(t,`She is ${art(c.nat)} ${c.nat} girl. She is from ____.`,N(c),sample(C,6).map(N)))});
 else if(t=='irregular')IRR.forEach(([a,b,c])=>{o.push(mk(t,`What is the past simple (V2) of "<b>${a}</b>"?`,b,[a,a+'ed',c,a+'en',a+'s']));o.push(mk(t,`What is the past participle (V3) of "<b>${a}</b>"?`,c,[a,b,a+'ed',a+'en',a+'s']))});
 else WL.forEach(w=>o.push(mk(t,`${w.e} What is the meaning of "<b>${w.w}</b>"?`,w.fa,sample(WL,6).map(x=>x.fa))));
 return o}
function dt(t){const r=[];
 if(['simple_present','present_continuous','simple_past','future'].includes(t))V.forEach(v=>SUBJ.forEach(S=>{const f=t=='simple_present'?(is3(S)?v.s:v.v):t=='present_continuous'?v.g:t=='simple_past'?v.p:'will '+v.v;
  r.push([f,t=='present_continuous'?`${S} ${be(S)} ${v.g}`:t=='future'?`${S} will ${v.v}`:`${S} ${f}`,sent(t,v,S,'p')])}));
 else if(t=='to_be')SUBJ.forEach(S=>[0,1].forEach(p=>{const f=be(S,p);r.push([f,`${S} ${f}`,`${S} ${f} at home ${p?'yesterday':'now'}.`])}));
 else if(t=='countries')C.forEach(c=>r.push([c.n,'from '+N(c),`He is from ${N(c)}.`]));
 else if(t=='nationalities')C.forEach(c=>r.push([c.nat,`${art(c.nat)} ${c.nat} student`,`She is ${art(c.nat)} ${c.nat} student.`]));
 else if(t=='irregular')IRR.forEach(([a,b])=>r.push([b,`${a} ${b}`,`The past form of ${a} is ${b}.`]));
 else WL.forEach(x=>r.push([x.w,`${art(x.w)} ${x.w}`,`I see ${art(x.w)} ${x.w}.`]));
 return r}
function dictItems(t,l){const d=dt(t),pools=[0,1,2].map(i=>uniq(d.map(x=>x[i]))),order=[l,...[0,1,2].filter(i=>i!=l)];let out=[];
 order.forEach(i=>{if(out.length<10)out=out.concat(sample(pools[i].filter(x=>!out.includes(x)),10-out.length))});
 return out.map(s=>({type:'dict',t,s,id:'d|'+t+s}))}
/* ---------- LESSONS ---------- */
const ex=(t,k,off,n)=>V.slice(off,off+n).map((v,i)=>[k=='p'?v.e:k=='n'?'🚫':'❓',sent(t,v,SUBJ[(i+off+(k=='p'?0:1))%6],k)]);
const L={
to_be:{n:'Verb To Be',fa:'فعل to be یعنی «بودن». برای معرفی خود، توصیف و مکان استفاده می‌شود. حال: am / is / are — گذشته: was / were.',en:'The verb "to be" describes who or what someone is, where they are, and how they feel.',
 f:['I am · You are · He/She/It is · We/They are','Past: I/He/She/It was · You/We/They were','(−) S + be + not   (?) Be + S ... ?'],
 u:['معرفی: I am a student.','حالت و ویژگی: She is happy.','مکان: They are at school.','گذشته: It was rainy yesterday.'],
 tip:['I فقط با am می‌آید؛ You همیشه are/were.','در سؤال، فعل بودن قبل از فاعل می‌آید: Is she a doctor?'],
 err:[['She are happy.','She is happy.'],['I is a student.','I am a student.'],['They was late.','They were late.']],
 ex:[['🙋','I am a student.'],['👦','He is tall.'],['👧','She is happy.'],['🐱','It is small.'],['👫','We are friends.'],['🏫','They are at school.'],['🌧️','It was rainy yesterday.'],['😴','I was tired last night.'],['⏰','You were late.'],['🎉','We were at the party.']],
 nq:[['🚫','I am not a teacher.'],['🚫','They were not at home.'],['❓','Is she a doctor?'],['❓','Were you at school yesterday?']]},
simple_present:{n:'Simple Present',fa:'برای عادت‌ها، کارهای تکراری و حقایق همیشگی. برای He / She / It به آخر فعل s یا es اضافه می‌شود.',en:'We use the simple present for habits, routines and facts. Add -s / -es for he, she, it.',
 f:['(+) S + V1 (he/she/it → V1 + s/es)','(−) S + do/does + not + V1','(?) Do/Does + S + V1 ... ?'],
 u:['عادت: I play football every day.','حقیقت: The sun rises in the east.','برنامه ثابت: The train leaves at 8.'],
 tip:['فعل‌های ‑s ‑sh ‑ch ‑x ‑o → es: watches, goes.','حرف بی‌صدا + y → ies: study → studies.','بعد از does فعل ساده می‌آید: Does she play?'],
 err:[['She play football.','She plays football.'],['Does she plays?','Does she play?'],['He don\'t like tea.','He doesn\'t like tea.']]},
present_continuous:{n:'Present Continuous',fa:'برای کاری که همین الان در حال انجام است. ساختار: am / is / are + فعل با ing.',en:'We use the present continuous for actions happening now.',
 f:['(+) S + am/is/are + V-ing','(−) S + am/is/are + not + V-ing','(?) Am/Is/Are + S + V-ing ... ?'],
 u:['الان: He is running.','همین حالا: They are playing football.','زمان‌نماها: now, at the moment, right now.'],
 tip:['run → running (حرف آخر دوبار)، make → making (e حذف می‌شود).','فعل‌های حالتی مثل know و like معمولاً ing نمی‌گیرند.'],
 err:[['He running.','He is running.'],['I am play.','I am playing.'],['They is eating.','They are eating.']]},
simple_past:{n:'Simple Past',fa:'برای کاری که در گذشته شروع شده و تمام شده است. فعل باقاعده: ed می‌گیرد (played). فعل بی‌قاعده: شکل خاص V2 (go → went). بعد از did و didn\'t فعل به V1 برمی‌گردد.',en:'We use the simple past for finished actions. After did / did not, the verb goes back to V1.',
 f:['(+) S + V2   (I played football yesterday.)','(−) S + did not + V1   (I did not play football.)','(?) Did + S + V1 ... ?   (Did you play football?)'],
 u:['کار تمام‌شده: She went to school.','زمان‌نماها: yesterday, last week, two days ago.'],
 tip:['Regular: play → played، study → studied، stop → stopped.','Irregular: go → went، buy → bought، see → saw (جدول Irregular Verbs).','در منفی و سؤال، did کار گذشته را انجام می‌دهد؛ پس فعل V1 است.'],
 err:[['She goed to school.','She went to school.'],['Did you went?','Did you go?'],['I didn\'t played.','I didn\'t play.']]},
future:{n:'Future: Will & Be Going To',fa:'will برای تصمیم لحظه‌ای، قول و پیش‌بینی است. be going to برای برنامه‌ای که از قبل تصمیمش را گرفته‌ای یا وقتی نشانه‌ای می‌بینی.',en:'Use "will" for quick decisions, promises and predictions. Use "be going to" for plans and evidence.',
 f:['will: S + will + V1   (I will travel.)','(−) S + will not (won\'t) + V1   (?) Will + S + V1 ... ?','be going to: S + am/is/are + going to + V1'],
 u:['تصمیم لحظه‌ای: I\'m cold. I will close the window.','برنامه: I am going to study tonight.','نشانه: Look at the clouds! It is going to rain.'],
 tip:['بعد از will همیشه V1 می‌آید.','تفاوت: will = تصمیم همین الان؛ going to = برنامه از قبل.'],
 err:[['She will studies.','She will study.'],['I am going study.','I am going to study.'],['He will to go.','He will go.']]}};
/* ---------- STATE / ROUTER ---------- */
let R=null,cur='home';const P={},A={};
const NAV=[['home','🏠','Home'],['grammar','📚','Grammar'],['dict','✍️','Dictation'],['exam','📝','Exam'],['prog','📊','Progress'],['set','⚙️','Settings']];
function go(p,q){if(!D.name)p='login';cur=p;P[p](q);$('#nav').innerHTML=D.name?NAV.map(n=>`<button class="${n[0]==cur?'on':''}" data-a="go" data-p="${n[0]}"><b>${n[1]}</b>${n[2]}</button>`).join(''):'';
 $('#top').innerHTML=D.name?`<span class="chip en">Hello ${esc(D.name)} 👋</span><span class="chip en">Level ${lv()} · XP ${D.xp.toLocaleString('en')}</span><button class="sp" data-a="tg" aria-label="Dark / Light mode">🌓 Dark / Light</button>`:''}
const view=h=>{$('#app').innerHTML=h;scrollTo(0,0)};
const back=(to='home')=>`<button class="btn2" data-a="go" data-p="${to}">← Back</button>`;
const sel=(id,o)=>`<select id="${id}">${Object.entries(o).map(([k,v])=>`<option value="${k}">${v}</option>`).join('')}</select>`;
const exCard=([e,s])=>`<div class="ex"><span class="em">${e}</span><span class="en" style="flex:1">${s}</span>${sp(s)}</div>`;
P.login=()=>view(`<div class="card" style="max-width:420px;margin:12vh auto;text-align:center"><div class="big">🎓</div><h1 class="en">ENGLISH_PAYAM_GHADIR</h1><h2 style="margin:0">پیام غدیر</h2><p class="mu">کلاس هشتم · معلم: آقای محمدی</p><p>Enter your name / اسمت را وارد کن</p><input id="nm" class="in" maxlength="30" placeholder="Name / نام"><button class="btn" data-a="login">Enter / ورود</button></div>`);
P.home=()=>{const T=[['grammar','📚','Grammar'],['countries','🌍','Countries'],['dict','✍️','Dictation'],['vocab','🧠','Vocabulary'],['irr','🔤','Irregular Verbs'],['daily','🏆','Daily Challenge'],['exam','📝','Exam Mode'],['prog','📊','My Progress'],['mis','⭐','My Mistakes']];
 const nx=Math.pow(lv(),2)*100,pv=Math.pow(lv()-1,2)*100;
 view(`<div class="card" style="text-align:center"><b>پیام غدیر</b> <span class="en mu">· ENGLISH_PAYAM_GHADIR</span><div class="mu">کلاس هشتم · معلم: آقای محمدی</div></div><div class="hi">سلام ${esc(D.name)} 👋<br><span class="en">Welcome, ${esc(D.name)}!</span></div><div class="card"><div class="en">Level ${lv()} · XP ${D.xp.toLocaleString('en')} / ${nx.toLocaleString('en')}</div><div class="bar"><i style="width:${Math.min(100,(D.xp-pv)/(nx-pv)*100)}%"></i></div></div><div class="grid">${T.map(t=>`<button class="tile" data-a="go" data-p="${t[0]}"><b>${t[1]}</b><span class="en">${t[2]}</span></button>`).join('')}</div>`)};
P.grammar=()=>view(`<h2>📚 Grammar</h2><div class="grid">${GT.map(t=>`<button class="tile" data-a="go2" data-p="${t}"><b>${t=='to_be'?'🙋':ex(t,'p',0,1)[0]?.[0]||'📘'}</b><span class="en">${L[t].n}</span>${D.done.includes(t)?'<span class="badge">✓</span>':''}</button>`).join('')}</div><p class="mu">درس‌های بیشتر (Pronouns، Prepositions، …) در نسخه‌های بعدی اضافه می‌شوند.</p>`);
P.lesson=t=>{const l=L[t],e=l.ex||ex(t,'p',0,10),nq=l.nq||[...ex(t,'n',10,2),...ex(t,'q',12,2)];
 view(`${back('grammar')}<h2 class="en">${l.n}</h2><div class="card"><p>${l.fa}</p><p class="en mu">${l.en}</p></div><h3>Formula</h3><div class="card en fm">${l.f.map(x=>`<div>${x}</div>`).join('')}</div>
 <h3>کاربردها</h3><div class="card"><ul>${l.u.map(x=>`<li>${x}</li>`).join('')}</ul></div><h3>نکته‌ها</h3><div class="card"><ul>${l.tip.map(x=>`<li>${x}</li>`).join('')}</ul></div>
 <h3>اشتباهات رایج</h3><div class="card en">${l.err.map(x=>`<div><span class="bad">✗ ${x[0]}</span> → <span class="good">✓ ${x[1]}</span></div>`).join('')}</div>
 <h3>Examples (+)</h3><div class="grid" style="grid-template-columns:repeat(auto-fill,minmax(260px,1fr))">${e.map(exCard).join('')}</div>
 <h3>Negative &amp; Question</h3><div class="grid" style="grid-template-columns:repeat(auto-fill,minmax(260px,1fr))">${nq.map(exCard).join('')}</div>
 <div class="row"><button class="btn" data-a="lq" data-p="${t}">📝 Quiz (10)</button></div>`)};
P.irr=(f='')=>{view(`${back()}<h2>🔤 Irregular Verbs</h2><input id="sq" class="in en" placeholder="Search / جستجو…" value="${esc(f)}"><div class="card" style="overflow-x:auto"><table class="en"><tr><th>V1</th><th>V2</th><th>V3</th><th>معنی</th></tr>${IRR.filter(r=>r.join(' ').toLowerCase().includes(f.toLowerCase())).map(r=>`<tr>${[0,1,2].map(i=>`<td>${r[i]} ${sp(r[i].split('/')[0])}</td>`).join('')}<td dir="rtl">${r[3]}</td></tr>`).join('')}</table></div>`);const i=$('#sq');i.focus();i.setSelectionRange(99,99)};
P.countries=(f='')=>{view(`${back()}<h2>🌍 Countries</h2><input id="cq" class="in en" placeholder="Search country… / جستجوی کشور" value="${esc(f)}"><div class="grid">${C.filter(c=>c.n.toLowerCase().includes(f.toLowerCase())||c.nat.toLowerCase().includes(f.toLowerCase())).map(c=>`<button class="tile" data-a="ctry" data-p="${c.n}"><b>${c.f}</b><span class="en">${c.n}</span></button>`).join('')}</div>`);const i=$('#cq');i.focus();i.setSelectionRange(99,99)};
P.country=n=>{const c=C.find(x=>x.n==n);view(`${back('countries')}<div class="card en"><div class="big">${c.f}</div><h2>${c.n} ${sp(c.n)}</h2><table><tr><td>Country</td><td>${c.n}</td></tr><tr><td>Nationality</td><td>${c.nat} ${sp(c.nat)}</td></tr><tr><td>Language</td><td>${c.l}</td></tr><tr><td>Capital</td><td>${c.cap} ${sp(c.cap)}</td></tr><tr><td>Area</td><td>≈ ${Math.round(c.a*1000).toLocaleString('en')} km²</td></tr><tr><td>Population</td><td>≈ ${c.p>=100?Math.round(c.p):c.p} million (2023, approx.)</td></tr></table><p>He is from ${N(c)}. He is ${c.nat}. ${sp(`He is from ${N(c)}. He is ${c.nat}.`)}</p></div><button class="btn" data-a="cq">📝 Country &amp; Nationality quiz</button>`)};
P.vocab=(k='Family')=>view(`${back()}<h2>🧠 Vocabulary</h2><div class="row">${Object.keys(W).map(x=>`<button class="${x==k?'btn':'btn2'}" data-a="go2v" data-p="${x}">${x}</button>`).join('')}</div><div class="grid" style="margin-top:12px">${W[k].map(w=>`<div class="card en" style="text-align:center"><div class="big">${w.e}</div><b>${w.w}</b> ${sp(w.w)}<div dir="rtl" class="mu">${w.fa}</div><div class="mu">It is ${art(w.w)} ${w.w}. ${sp(`It is ${art(w.w)} ${w.w}.`)}</div></div>`).join('')}</div><div class="row"><button class="btn" data-a="vq">📝 Vocabulary quiz</button></div>`);
P.dict=()=>view(`${back()}<h2>✍️ Dictation</h2><div class="card"><p>موضوع و سطح را انتخاب کن. هر آزمون ۱۰ سؤال دارد و فقط از همان موضوع است.</p>${sel('tp',TP)} ${sel('lv',{0:'Easy (Words)',1:'Medium (Phrases)',2:'Hard (Sentences)'})}<div class="row"><button class="btn" data-a="dstart">Start</button></div></div>`);
P.exam=()=>view(`${back()}<h2>📝 Exam Mode</h2><div class="card">${sel('tp',TP)} ${sel('cn',{10:'10 Questions',20:'20 Questions',30:'30 Questions'})}<div class="row"><button class="btn" data-a="estart">Start exam</button></div></div>`);
P.daily=()=>{const g=sample(GT,2);run([...sample(Q(g[0]),1),...sample(Q(g[1]),1),...sample(Q('vocabulary'),2),...dictItems(sample(GT,1)[0],2).slice(0,1)],'Daily Challenge','daily')};
P.mis=()=>{const a=D.mis.filter(m=>!m.m);view(`${back()}<h2>⭐ My Mistakes</h2><div class="card">${a.length?`<button class="btn" data-a="mpr">Practice My Mistakes (${a.length})</button>`:'<p>هنوز اشتباهی ثبت نشده — یا همه Mastered شده‌اند 🎉</p>'}</div>${D.mis.map(m=>`<div class="card en">${m.m?'<span class="badge">Mastered ✅</span> ':''}<b>${m.type=='dict'?'🎧 '+m.s:m.q}</b><div class="mu">${TP[m.t]} · ${m.c}/3</div></div>`).join('')}`)};
P.prog=()=>{const st=Object.entries(D.st),avg=a=>a.length?Math.round(a.reduce((s,x)=>s+x.p,0)/a.length)+'%':'—',pc=t=>D.st[t]?Math.round(D.st[t].c/D.st[t].n*100):0;
 view(`${back()}<h2>📊 My Progress</h2><div class="grid"><div class="card en"><b>${D.xp.toLocaleString('en')}</b><div class="mu">Total XP</div></div><div class="card en"><b>${lv()}</b><div class="mu">Level</div></div><div class="card en"><b>${D.done.length}/${GT.length}</b><div class="mu">Lessons completed</div></div><div class="card en"><b>${avg(D.di)}</b><div class="mu">Dictation avg</div></div><div class="card en"><b>${avg(D.ex)}</b><div class="mu">Exam avg</div></div></div>
 <div class="card"><h3>Accuracy by topic</h3>${Object.keys(TP).map(t=>`<div class="en">${TP[t]} — ${pc(t)}%${D.st[t]?` (${D.st[t].n} answers)`:''}</div><div class="bar" style="margin-bottom:8px"><i style="width:${pc(t)}%"></i></div>`).join('')}</div>
 <div class="card en"><h3>Recent exams</h3>${D.ex.slice(-5).reverse().map(x=>`<div>${TP[x.t]} — ${x.p}%</div>`).join('')||'—'}<h3>Recent dictations</h3>${D.di.slice(-5).reverse().map(x=>`<div>${TP[x.t]} — ${x.p}%</div>`).join('')||'—'}</div>`)};
P.set=()=>view(`${back()}<h2>⚙️ Settings</h2><div class="card"><label>نام / Name</label><input id="nm" class="in" value="${esc(D.name)}"><button class="btn" data-a="rename">Save name</button></div>
 <div class="card"><label>Theme</label><br>${sel('th',{auto:'Auto',light:'☀️ Light',dark:'🌙 Dark'})} <label>Audio speed</label> ${sel('rt',{0.75:'0.75x',1:'1x',1.25:'1.25x'})} <button class="sp" data-t="Hello! This is the audio test.">🔊 Test</button></div>
 <div class="card"><button class="btn2 bad" data-a="reset">Reset Progress</button></div>`);
/* ---------- QUIZ RUNNER (mc + dictation) ---------- */
const norm=s=>s.toLowerCase().replace(/[.,!?'"\-]/g,' ').replace(/\s+/g,' ').trim();
function run(items,title,mode,t){R={items,i:0,res:[],t0:Date.now(),title,mode,t,lock:0,hint:0};rq()}
function rq(){const it=R.items[R.i],n=R.items.length;cur=R.mode;
 view(`<div class="bar"><i style="width:${R.i/n*100}%"></i></div><p class="mu en">${R.title} · ${R.i+1}/${n}</p>`+(it.type=='dict'?`<div class="card" style="text-align:center"><div class="big">🎧</div><button class="btn" data-a="again">🔊 Listen Again</button><input id="ans" class="in en" autocomplete="off" autocapitalize="off" spellcheck="false" placeholder="Type what you hear…"><p id="hint" class="mu en"></p><div class="row" style="justify-content:center"><button class="btn2" data-a="hint">💡 Hint (−5 XP)</button><button class="btn" data-a="sub">➡️ Next</button></div></div>`:`<div class="card"><p class="q en">${it.q}</p><div class="opts">${it.o.map((o,k)=>`<button class="opt en" data-a="pick" data-p="${k}">${o}</button>`).join('')}</div><div id="fb"></div></div>`));
 R.lock=0;R.hint=0;if(it.type=='dict'){setTimeout(()=>say(it.s),300);$('#ans').focus()}}
function rec(it,ok,given,hint){const s=D.st[it.t]=D.st[it.t]||{c:0,n:0};s.n++;if(ok){s.c++;D.xp+=hint?5:10}
 let m=D.mis.find(x=>x.id==it.id);
 if(ok&&m){m.c++;if(m.c>=3)m.m=true}else if(!ok){if(m){m.c=0;m.m=false}else D.mis.push({...it,c:0,m:false})}
 R.res.push({it,ok,given});save()}
A.pick=k=>{if(R.lock)return;R.lock=1;const it=R.items[R.i],ok=it.o[+k]==it.r;
 document.querySelectorAll('.opt').forEach((b,j)=>{if(it.o[j]==it.r)b.classList.add('ok');else if(j==+k)b.classList.add('no')});
 rec(it,ok,it.o[+k]);$('#fb').innerHTML=`<p class="${ok?'good':'bad'}">${ok?'✓ Correct! +10 XP':'✗ Correct answer: <b class=en>'+it.r+'</b>'}</p><button class="btn" data-a="nx">➡️ Next</button>`};
A.again=()=>say(R.items[R.i].s);
A.hint=()=>{R.hint=1;$('#hint').textContent=R.items[R.i].s.split(' ').map(w=>w[0]+'_'.repeat(w.length-1)).join(' ')};
A.sub=()=>{const it=R.items[R.i],g=$('#ans').value;rec(it,norm(g)==norm(it.s),g.trim(),R.hint);A.nx()};
A.nx=()=>{R.i++;R.i>=R.items.length?fin():rq()};
const GR=k=>k>=10?['A+ 🌟','عالی! بی‌نقص بود!']:k==9?['A+','فوق‌العاده!']:k==8?['A','خیلی خوب!']:k==7?['B+','آفرین، ادامه بده!']:k==6?['B','خوب است؛ کمی تمرین بیشتر']:k==5?['C','قابل قبول؛ تمرین کن']:['Needs Practice','نگران نباش؛ دوباره تلاش کن 💪'];
function fin(){const n=R.items.length,c=R.res.filter(r=>r.ok).length,p=Math.round(c/n*100),g=GR(Math.round(c/n*10)),sec=Math.round((Date.now()-R.t0)/1000),bad=R.res.filter(r=>!r.ok);let bonus='';
 if(c==n&&n>=10&&R.mode!='mis'){D.xp+=50;bonus='<p class="good">Perfect! +50 XP 🏆</p>'}
 if(R.mode=='daily'){const d=new Date().toDateString();if(D.dc!=d){D.dc=d;D.xp+=30;bonus='<p class="good">Daily Challenge Completed! 🎉 +30 XP</p>'}else bonus='<p class="mu">Daily Challenge Completed! 🎉 (XP already earned today)</p>'}
 if(R.mode=='exam')D.ex.push({t:R.t,p});if(R.mode=='dict')D.di.push({t:R.t,p});
 if(R.mode=='lesson'&&p>=70&&!D.done.includes(R.t)){D.done.push(R.t);bonus+='<p class="good">Lesson completed ✅</p>'}save();go2();
 view(`<div class="card" style="text-align:center"><h2 class="en">${R.mode=='dict'?'DICTATION':'QUIZ'} RESULT</h2><div class="big en">${c} / ${n}</div><h2 class="en">${g[0]}</h2><p>${g[1]}</p>${bonus}<div class="en mu">Correct: ${c} · Wrong: ${n-c} · Accuracy: ${p}% · Time: ${Math.floor(sec/60)}:${String(sec%60).padStart(2,'0')}</div></div>
 ${bad.map(r=>`<div class="card en"><div class="mu">${r.it.type=='dict'?'You wrote:':r.it.q}</div><div class="bad">${r.it.type=='dict'?(r.given||'(empty)'):'✗ '+r.given}</div><div class="mu">Correct:</div><div class="good">${r.it.type=='dict'?r.it.s:r.it.r}</div></div>`).join('')}
 <div class="row">${bad.length?'<button class="btn" data-a="mpr">Practice My Mistakes</button>':''}<button class="btn2" data-a="go" data-p="home">Home</button></div>`)}
const go2=()=>{};
/* ---------- ACTIONS ---------- */
A.tg=()=>{const d=document.documentElement.dataset.theme=='dark'||(D.theme=='auto'&&matchMedia('(prefers-color-scheme: dark)').matches);D.theme=d?'light':'dark';save();theme();const s=$('#th');if(s)s.value=D.theme};A.go=p=>go(p);A.go2=t=>go('lesson',t);A.go2v=k=>go('vocab',k);A.ctry=n=>go('country',n);
A.login=()=>{const n=$('#nm').value.trim();if(n){D.name=n;save();go('home')}};
A.rename=()=>{const n=$('#nm').value.trim();if(n){D.name=n;save();go('set')}};
A.lq=t=>run(sample(Q(t),10),L[t].n,'lesson',t);
A.cq=()=>run(sample(Q('nationalities'),10),'Country & Nationality','quiz','nationalities');
A.vq=()=>run(sample(Q('vocabulary'),10),'Vocabulary','quiz','vocabulary');
A.dstart=()=>{const t=$('#tp').value;run(dictItems(t,+$('#lv').value),'Dictation · '+TP[t],'dict',t)};
A.estart=()=>{const t=$('#tp').value;run(sample(Q(t),+$('#cn').value),'Exam · '+TP[t],'exam',t)};
A.mpr=()=>{const a=D.mis.filter(m=>!m.m).slice(0,10);if(a.length)run(a.map(m=>m.type=='mc'?{...m,o:sh(m.o)}:m),'My Mistakes','mis','mis')};
A.reset=()=>{if(confirm('Reset all progress? / همه پیشرفت پاک شود؟')){try{localStorage.removeItem('epq_d')}catch(e){}location.reload()}};
document.addEventListener('click',e=>{const b=e.target.closest('[data-a],.sp');if(!b)return;if(b.dataset.a)A[b.dataset.a](b.dataset.p);else say(b.dataset.t)});
document.addEventListener('input',e=>{if(e.target.id=='sq')P.irr(e.target.value);if(e.target.id=='cq')P.countries(e.target.value)});
document.addEventListener('change',e=>{if(e.target.id=='th'){D.theme=e.target.value;save();theme()}if(e.target.id=='rt'){D.rate=+e.target.value;save()}});
document.addEventListener('keydown',e=>{if(e.key=='Enter'){if(e.target.id=='ans')A.sub();else if(e.target.id=='nm')cur=='login'?A.login():A.rename()}});
const theme=()=>D.theme=='auto'?document.documentElement.removeAttribute('data-theme'):document.documentElement.dataset.theme=D.theme;
const _s=P.set;P.set=()=>{_s();$('#th').value=D.theme;$('#rt').value=D.rate};
theme();go('home');
</script></body></html>
