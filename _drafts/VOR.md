---
layout: post
title: "Intro to VOR"
category: VOR
cat: Vestibulo-ocular reflex
---
Hello world!

Here\'s some ruby highlighting:
{% highlight ruby linenos=table %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}


... and here's some matlab code:
{% highlight matlab linenos=table %}
W = [ 0.9 -0.4;
      0.4 0.9 ]

V = [1 ; 0]

tEnd = 100;
tVec = 0:tEnd;
nTs=tEnd+1;
x=zeros(1,nTs);
start=11
x(start)=1;

y=zeros(2,nTs);
for t=2:nTs,
    y(:,t) = W*y(:,t-1) + V*x(t-1);
end

clf;
plot(tVec, y)

[eVec, eVal] = eig(W);
eVal=diag(eVal);
magEVal = abs(eVal);
freq = angle(eVal) / (2 * pi);
[eVec eVal magEVal freq]
{% endhighlight %}


And here is an image:
![Vestibulo-ocular reflex](/images/VOR.png)  