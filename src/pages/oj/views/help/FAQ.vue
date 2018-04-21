<template>
  <panel>
    <div slot="title">经常被问到的问题</div>
    <div class="content markdown-body">
      <ul>
        <li>输入和输出在哪里?
          <p>你的程序将从 <code>stdin</code>('标准输入') 写入输出到 <code>stdout</code>('标准输出'')。
            例如，你可以用 <code>scanf</code> 在 C 或 <code>cin</code> C++ 中使用从stdin读取,并用 <code>printf</code> 在 C 或 <code>cout</code> C++ 中使用以写入stdout。
            用户程序不允许读取或写入文件，否则您将得到一个 <code>Runtime Error</code>.
          </p>
        </li>
        <li>提交执行时间的含义是什么?
        <p>onlinejudge可能会使用不同的输入文件多次测试您的代码。如果你的代码在每个输入文件的时限内给出了正确的答案，那么显示的执行  时间就是每个测试用例花费的时间的最大值。否则，执行时间将毫无意义。
        </p>
        </li>
        <li>我如何使用C++ Int64?
          <p>你应该声明为 <code>long long</code> 和使用e with <code>cin/cout</code> 或 <code>%lld</code>, 使用<code> __int64</code> 将导致 <code>Compile Error</code>。</p>
        </li>
        <li>Java 规范?
          <p>所有程序都必须以一个 <code>Main</code> 类中的静态主方法开始。 不要使用公共类: 甚至 <code>Main</code> 必须是非公开的，以避免编译错误。使用缓冲的I / O来避免由于过度冲刷而超过时间限制。</p>
        </li>
        <li>关于表示错误?
          <p>在这个oj中没有表示错误。裁判将删减空格并包裹在输出的<b>最后</b>一行。
            如果它与正确的输出仍然不同，结果将是 <code>Wrong Answer</code>。</p>
        </li>
        <li>如何提交关于这个oj的错误？?
          <p>onlinejudge是开源的，你可以在<a href="https://github.com/orangeLQY">Github</a>提交问题。
          有关错误的详细信息（如env，version ..）是必需的，这将帮助我们解决错误。当然，我们很高兴合并你的拉请求。
          </p>
        </li>
      </ul>
    </div>
  </panel>
</template>

<script>
</script>

<style lang="less" scoped>
  .content {
    font-size: 16px;
    margin: 0 50px 40px 50px;
    > ul {
      list-style: disc;
      li {
        font-size: 16px;
        margin-top: 20px;
        &:first-child {
          margin-top: 0;
        }
        p {
          font-size: 14px;
          margin-top: 5px;
        }
      }
    }
  }
</style>
