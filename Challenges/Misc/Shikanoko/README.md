# しかのこのこのここしたんたん

ok so the MarkovChain.tsx in `dist` (given to you) and in `src` (actually being hosted) is slightly different (mainly cause I wanted to discourage people from reverse-engineering the flag from the client. I tried.)

## full writeup: https://rwandi-ctf.github.io/BlahajCTF2024/shikanokonokonoko/

## Solution

ok this is a very smoked challenge

I supposed step 1 is to realise that clicking the circles sets the state (calls `setState`) which updates `shistory`

So you just need to click those buttons...

I just wrote a puppeteer script to do it, you can find it in `/sol`:

honestly im sure there is a way to do this without using a puppeteer, like you could probably:
- open like 50 websites and wait
- somehow reverse-engineer the compiled react code (which I secretly modified) to get the flag

also I got slightly mentally insane from testing this
