<h1> Array methods </h1>

<div>
<p style="color:red;"> it is string method :)</p>
<h2>1- string to array</h2>
  <code>variable = "1,2,4,4";</code>
  <ul>
    <li>
    <code>
    <b>js</b> -> String.prototype.split(string) => variable = variable.split('');
    </code>
    </li>
    <li>
      <code>
        <b>php</b>-> explode($string,$array) => $variable = explode(',',$variable); 
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">variable => [1,2,3,4]</p>
</div>

<div>
  <h2>2- array to string</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.prototype.join(string) => variable = variable.join('!');
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => implode($string,$array)  =>   variable = implode('!',  $variable);
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">variable => 1!2!3!4</p>
</div>

<div>
  <h2>3- array size</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.length => variable.length;
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => count($array)  =>   count($variable);
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">sizes => 4</p>
</div>

<div>
  <h2>4- is array</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.isArray(array) => $isArr = Array.isArray(variable);
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => is_array($array)  => isArr = is_array($variable);
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">isArr => true</p>
</div>

<div>
  <h2>5- array reverse</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.prototype.reverse() => variable.reverse();
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => rsort($array) => rsort($variable);
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">variable => [4,4,2,1]</p>
</div>

<div>
  <h2>6- array reduce</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => reduce(callbackFunc,accumulator) => 
        x = variable.reduce(function(x,y) {
                return x+y;
              },0) ;
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => array_reduce($array,callbackFunc,$accumulator) => 
        $x = array_reduce($variable,function($x,$y) {
                  return x+y;
                },0) ;
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">x => 11</p>
</div>

<div>
  <h2>7- array splice</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.prototype.splice(start,length,[newVal,...]) =>
        x = variable.splice(0,2,['arif','x']);
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => array_splice($array,$start,$length,[$newVal,...]) => 
        $x = array_splice($variable,0,2,['arif','x']);
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">
  variable => ['arif','x',4,4] &nbsp x = [1,2]
  </p>
</div>

<div>
  <h2>8- array slice</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.prototype.slice(start,end) => x = variable.slice(1,2)
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => array_slice($array,$start,$length) => 
        $x = array_slice($variable,1,2)
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result js => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">x => [2]</p>
  <h3 style="color:tomato; display:inline-block;">Result php => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">x => [2,4]</p>
</div>

<div>
  <h2>9- array sort</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.prototype.sort(callbackFunc) => 
              x = variable.sort(function(x,y){ 
                return x-y;
              })
      </code>
    </li>
    <li>
      <h2>those are php sort methods
      </h2>
      <a href="https://www.php.net/manual/en/array.sorting.php">Click for more info</a>
      <ul><li>uasort</li><li>uksort</li><li>usort</li><li>sort</li><li>ksort</li><li>krsort</li><li>arsort</li><li>rsort</li></ul>
      <code>
        <b>php</b> => sort($array) => sort($variable)
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">x = [1,2,4,4]</p>
</div>

<div>
  <h2>10- array push</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.prototype.push(value, ...) => variable.push(2,2,2);
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => array_push($array,$value, ...)  => array_push($variable,2,2,2);
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">
  variable => [1,2,4,4,2,2,2] 
  </p>
</div>

<div>
  <h2>11- array pop</h2>
  <code>variable = [1,2,4,4];</code>
  <ul>
    <li>
      <code>
        <b>js</b> => Array.prototype.pop() = variable.pop()
      </code>
    </li>
    <li>
      <code>
        <b>php</b> => array_pop($array) => array_pop($variable);
      </code>
    </li>
  </ul>
  <h3 style="color:tomato; display:inline-block;">Result => </h3>
  <p style="border:#ffe500 solid 1px; display:inline-block; padding:5px; color:#11c125;">
  variable => [1,2,4]
   </p>
</div>