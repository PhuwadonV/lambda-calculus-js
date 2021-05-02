- [Example](https://jsfiddle.net/PhuwadonV/5zur1ady)
- [Lazy](https://jsfiddle.net/PhuwadonV/aL6xbu2d/)
```js
const TRUE = a => b => a;
const FALSE = a => b => b;
const NOT = a => a(b => c => c)(b => c => b);
const AND = a => b => a(b)(a);
const OR = a => b => b(b)(a);
const ZERO = a => b => b;
const IS_ZERO = a => a(b => c => d => d)(b => c => b);
const SUCC = a => b => c => b(a(b)(c))
const PRED = a => b => c => a(d => e => e(d(b)))(d => c)(d => d);
const PLUS = a => b => c => d => a(c)(b(c)(d));
const MULT = a => b => c => a(b(c));
const COMPOSE = a => b => c => a(b(c))
const IF = a => b => c => a(b)(c)
const NIL = a => b => b;
const IS_NIL = a => a(b => c => d => e => e)(b => c => b);
const CONS = a => b => c => d => c(a)(b(c)(d));
const HEAD = a => a(b => c => b)(b => c => c);
const TAIL = a => b => c => a(d => e => f => f(d)(e(b)))(d => c)(d => e => e);
const Y = a => (b => a(b(b)))(b => a(b(b)));
const Z = a => (b => a(c => b(b)(c)))(b => a(c => b(b)(c)));
```
