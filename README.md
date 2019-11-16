#实验报告
##实验目的
#####掌握字符串String及其方法的使用
#####掌握异常处理结构
##核心代码及注释
```javascript

	try{
		char[] chars = w.toCharArray();//定义数组
		StringBuffer y = new StringBuffer();//追加内容到当前StringBuffer对象的末尾
		//计算字符串中关键字出现的次数
		countString(w,"无");
		int i;
		for (i =0; i <chars.length; i++) {
			//在被选元素的结尾插入符号
			y.append(chars[i]);
			if ((i+1)%7==0&&(i+1)%2==1||(i+1)%14==0&&(i+1)%2==0) {
				//i%7等于0并且i为奇数时，在结尾加，
				if((i+1)%7==0&&(i+1)%2==1)
			y.append(",");	
				//i%14等于0并且i为偶数时，在结尾加。
				else
					y.append("。\n");
			}
			}
		System.out.println("<<长恨歌>>");
		System.out.println(y.toString());
	}
	catch(Exception e){
		System.out.println("发生异常："+e.toString());
	}	
	}
```
```javascript
	private static void countString(String w, String string) {
		// TODO Auto-generated method stub
		int count=0;
		while(w.indexOf(string)!=-1){//查找字串中指定字符首次出现的位置
			w = w.substring(w.indexOf(string)+1,w.length());    
            count++;
		}
		System.out.println(string+"出现的次数为:"+count+"次");
	}
```
##实验结果
`汉皇重色思倾国,御宇多年求不得。`
`杨家有女初长成,养在深闺人未识。`
`天生丽质难自弃,一朝选在君王侧。`
`回眸一笑百媚生,六宫粉黛无颜色。`
`春寒赐浴华清池,温泉水滑洗凝脂。`
`侍儿扶起娇无力,始是新承恩泽时。`
`云鬓花颜金步摇,芙蓉帐暖度春宵。`
`春宵苦短日高起,从此君王不早朝。`
`承欢侍宴无闲暇,春从春游夜专夜。`
`后宫佳丽三千人,三千宠爱在一身。`
`金屋妆成娇侍夜,玉楼宴罢醉和春。`
`姊妹弟兄皆列土,可怜光彩生门户。`
`遂令天下父母心,不重生男重生女。`
`骊宫高处入青云,仙乐风飘处处闻。`
`缓歌慢舞凝丝竹,尽日君王看不足。`
`渔阳鼙鼓动地来,惊破霓裳羽衣曲。`
`九重城阙烟尘生,千乘万骑西南行。`
`翠华摇摇行复止,西出都门百余里。`
`六军不发无奈何,宛转蛾眉马前死。`
`花钿委地无人收,翠翘金雀玉搔头。`
`君王掩面救不得,回看血泪相和流。`
`无出现的次数为:5`	
##实验感想
通过本次试验，我对字符串处理思想有了进一步的了解。
为一大段古诗填上标点符号，我运用了for循环，虽然做
的时候出现了错误，但在同学和老师的帮助下解决了问题。
我还加上了刚学的try...catch结构对异常进行捕捉和处理。
同时,在实验过程中,回顾书本上的理论知识,巩固了我的知识。	
