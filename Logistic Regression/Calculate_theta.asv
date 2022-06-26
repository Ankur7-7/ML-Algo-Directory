function [J_list, theta] = Calculate_theta(initial_theta, alpha, Max_iter)
%UNTITLED Summary of this function goes here
%   Detailed explanation goes here

theta = initial_theta;

a = load("ex2data1.txt");
X = [ones(length(a),1) a(:,1:2)];
y = a(:,3);

J_list = zeros(Max_iter,1);
for i=1:Max_iter

    [J, grad] = costFunction(theta, X, y);
    theta = theta - alpha*grad;
    J_list(i) = J;
end

end



