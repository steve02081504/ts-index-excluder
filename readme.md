# Ts-index-excluder

`Exclude<string, AnyLiteral>` is still `string`?  

💩not work:

```ts
interface cla {
	[key: Exclude<string, "b">]: cla;
	b(): void;
}
```

🥰work!

```ts
interface cla {
	b(): void;
	[key: `a${string}`]: cla;
	[key: `ba${string}`]: cla;
	[key: `bb${string}`]: cla;
	[key: `bc${string}`]: cla;
	[key: `bd${string}`]: cla;
	[key: `be${string}`]: cla;
	[key: `bf${string}`]: cla;
	[key: `bg${string}`]: cla;
	[key: `bh${string}`]: cla;
	[key: `bi${string}`]: cla;
	[key: `bj${string}`]: cla;
	[key: `bk${string}`]: cla;
	[key: `bl${string}`]: cla;
	[key: `bm${string}`]: cla;
	[key: `bn${string}`]: cla;
	[key: `bo${string}`]: cla;
	[key: `bp${string}`]: cla;
	[key: `bq${string}`]: cla;
	[key: `br${string}`]: cla;
	[key: `bs${string}`]: cla;
	[key: `bt${string}`]: cla;
	[key: `bu${string}`]: cla;
	[key: `bv${string}`]: cla;
	[key: `bw${string}`]: cla;
	[key: `bx${string}`]: cla;
	[key: `by${string}`]: cla;
	[key: `bz${string}`]: cla;
	[key: `bA${string}`]: cla;
	[key: `bB${string}`]: cla;
	[key: `bC${string}`]: cla;
	[key: `bD${string}`]: cla;
	[key: `bE${string}`]: cla;
	[key: `bF${string}`]: cla;
	[key: `bG${string}`]: cla;
	[key: `bH${string}`]: cla;
	[key: `bI${string}`]: cla;
	[key: `bJ${string}`]: cla;
	[key: `bK${string}`]: cla;
	[key: `bL${string}`]: cla;
	[key: `bM${string}`]: cla;
	[key: `bN${string}`]: cla;
	[key: `bO${string}`]: cla;
	[key: `bP${string}`]: cla;
	[key: `bQ${string}`]: cla;
	[key: `bR${string}`]: cla;
	[key: `bS${string}`]: cla;
	[key: `bT${string}`]: cla;
	[key: `bU${string}`]: cla;
	[key: `bV${string}`]: cla;
	[key: `bW${string}`]: cla;
	[key: `bX${string}`]: cla;
	[key: `bY${string}`]: cla;
	[key: `bZ${string}`]: cla;
	[key: `b0${string}`]: cla;
	[key: `b1${string}`]: cla;
	[key: `b2${string}`]: cla;
	[key: `b3${string}`]: cla;
	[key: `b4${string}`]: cla;
	[key: `b5${string}`]: cla;
	[key: `b6${string}`]: cla;
	[key: `b7${string}`]: cla;
	[key: `b8${string}`]: cla;
	[key: `b9${string}`]: cla;
	[key: `b_${string}`]: cla;
	[key: `c${string}`]: cla;
	[key: `d${string}`]: cla;
	[key: `e${string}`]: cla;
	[key: `f${string}`]: cla;
	[key: `g${string}`]: cla;
	[key: `h${string}`]: cla;
	[key: `i${string}`]: cla;
	[key: `j${string}`]: cla;
	[key: `k${string}`]: cla;
	[key: `l${string}`]: cla;
	[key: `m${string}`]: cla;
	[key: `n${string}`]: cla;
	[key: `o${string}`]: cla;
	[key: `p${string}`]: cla;
	[key: `q${string}`]: cla;
	[key: `r${string}`]: cla;
	[key: `s${string}`]: cla;
	[key: `t${string}`]: cla;
	[key: `u${string}`]: cla;
	[key: `v${string}`]: cla;
	[key: `w${string}`]: cla;
	[key: `x${string}`]: cla;
	[key: `y${string}`]: cla;
	[key: `z${string}`]: cla;
	[key: `A${string}`]: cla;
	[key: `B${string}`]: cla;
	[key: `C${string}`]: cla;
	[key: `D${string}`]: cla;
	[key: `E${string}`]: cla;
	[key: `F${string}`]: cla;
	[key: `G${string}`]: cla;
	[key: `H${string}`]: cla;
	[key: `I${string}`]: cla;
	[key: `J${string}`]: cla;
	[key: `K${string}`]: cla;
	[key: `L${string}`]: cla;
	[key: `M${string}`]: cla;
	[key: `N${string}`]: cla;
	[key: `O${string}`]: cla;
	[key: `P${string}`]: cla;
	[key: `Q${string}`]: cla;
	[key: `R${string}`]: cla;
	[key: `S${string}`]: cla;
	[key: `T${string}`]: cla;
	[key: `U${string}`]: cla;
	[key: `V${string}`]: cla;
	[key: `W${string}`]: cla;
	[key: `X${string}`]: cla;
	[key: `Y${string}`]: cla;
	[key: `Z${string}`]: cla;
	[key: `0${string}`]: cla;
	[key: `1${string}`]: cla;
	[key: `2${string}`]: cla;
	[key: `3${string}`]: cla;
	[key: `4${string}`]: cla;
	[key: `5${string}`]: cla;
	[key: `6${string}`]: cla;
	[key: `7${string}`]: cla;
	[key: `8${string}`]: cla;
	[key: `9${string}`]: cla;
	[key: `_${string}`]: cla;

}
```
